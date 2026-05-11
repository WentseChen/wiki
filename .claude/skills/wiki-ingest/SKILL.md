---
name: wiki-ingest
description: Ingest a blog / paper / open-source project into the wiki by URL. Fetches the page, drops a raw stub, updates compiled articles (topics, concepts, summaries, index). Use when the user says "add to wiki", "/wiki-ingest <url>", or hands you a link to remember.
user-invocable: true
allowed-tools:
  - WebFetch
  - Read
  - Write
  - Edit
  - AskUserQuestion
  - Bash(ls *)
  - Bash(grep *)
  - Bash(find *)
  - Bash(test *)
---

# /wiki-ingest — Add a URL to the wiki

This skill lives in-repo at `~/wiki/.claude/skills/wiki-ingest/`. It ships with the wiki, so it works on any machine that has the repo checked out.

## What it does

Given a URL, it:

1. Fetches the page.
2. Writes a raw stub at `raw/<type>/<slug>/README.md` (the README.md IS the raw file).
3. Writes a 1-paragraph summary at `articles/summaries/<slug>.md`.
4. Prepends a one-liner under `## Recent` in `articles/topics/<topic>.md` for each topic.
5. Auto-generates / appends to 0–3 `articles/concepts/<concept>.md` pages.
6. Prepends a one-liner under `## Recent additions` in `articles/index.md` (cap 20).

The `Stop` hook in `.claude/settings.json` then commits + pushes to `origin/main`.

## Working directory

Always `/zfsauton2/home/wentsec/wiki`. All paths below are repo-relative.

## Step 1 — get URL

URL is **mandatory**.

- If the user typed `/wiki-ingest <url>`, use that URL.
- If no URL was passed, ask via AskUserQuestion. Don't proceed without one.

## Step 2 — fetch

`WebFetch` the URL with a prompt like: "Extract: title, authors, year/date, venue (if any), 2–3 sentence abstract/takeaway, 3–5 key points, 2–3 specific named concepts/methods (e.g. PPO, MCTS, retrieval-augmented generation)."

If WebFetch fails (404, paywall, robots), tell the user and stop — don't fabricate the entry.

## Step 3 — classify type

- `arxiv.org/abs/*` or `arxiv.org/pdf/*` → `paper`
- `github.com/<org>/<repo>` (root) → `project`
- Otherwise → `blog`

If ambiguous (e.g. a Hugging Face page that's both a paper and a model card), ask the user.

## Step 4 — classify topics

Pick **1–3** from this fixed list, based on the fetched content:

`nlp · rl · agents · self-play · game-theory · multimodal · vision · systems · continuous-learning · theory · bandit · ml · others`

Use `others` only as a last resort.

## Step 5 — slug

- kebab-case from the title, ≤6 words, lowercase, ASCII only.
- Strip stopwords if needed for length, but keep it recognizable.
- Check `raw/<type>/` for collisions. If `<slug>` exists, try `<slug>-2`, `<slug>-3`, …

Example: "LLM Knowledge Bases" → `llm-knowledge-bases`.

## Step 6 — write raw entry

`raw/<type>/<slug>/README.md`:

```markdown
---
title: <title>
url: <url>
type: blog | paper | project
authors: [name1, name2]
venue: <conf/journal/org>      # omit if N/A
year: <YYYY>
topics: [<t1>, <t2>]
added: <YYYY-MM-DD>            # today
arxiv_id: <id>                 # papers only, omit if N/A
github: <org/repo>             # projects only, omit if N/A
---

# <title>

**Link:** <url>

## Summary
<1–3 paragraphs from the WebFetch result>

## Key points
- <bullet 1>
- <bullet 2>
- <bullet 3>

## See also
<!-- [[<related-slug>]] — optional, link if obvious relatives exist -->
```

Don't create `notes.md` or `images/` — they're optional and added on demand.

## Step 7 — write summary

`articles/summaries/<slug>.md`:

```markdown
# <title>

*<type>, <year>. <authors>.*

<1 short paragraph — what it is + why it matters>

→ [raw entry](../../raw/<type>/<slug>/README.md) · [url](<url>)
```

## Step 8 — update topic pages

For each topic in frontmatter, open `articles/topics/<topic>.md` and prepend a line directly under the `## Recent` heading:

```markdown
- [[<slug>]] — <one-line takeaway>. *<first-author et al.>, <year>.*
```

If the file has `<!-- newest at top — managed by /wiki-ingest -->` placeholder, insert above it.

## Step 9 — auto-generate concept pages

For each of the 0–3 named concepts the WebFetch returned:

- concept-slug = kebab-case of the concept name (e.g. `proximal-policy-optimization`, `ppo`, `mcts`).
- If `articles/concepts/<concept-slug>.md` does NOT exist, create:

  ```markdown
  # <concept name>

  <1–2 sentence definition — the LLM's best short gloss>

  ## Sources
  - [[<slug>]]
  ```

- If it exists, append `- [[<slug>]]` to the `## Sources` list (avoid duplicates).

This is what makes the wiki "compile" rather than just collect — concept pages become natural hubs over time.

## Step 10 — update index

Prepend the same one-liner from step 8 under `## Recent additions` in `articles/index.md`. Cap the list at 20 entries — drop the oldest if it would exceed.

## Step 11 — report

Print the list of created / edited file paths. End the turn — the `Stop` hook commits + pushes automatically.

## Failure modes / what NOT to do

- Don't write anything if WebFetch failed. Surface the error.
- Don't add `*.pdf` / `*.html` — the `.gitignore` blocks them anyway. Link only.
- Don't invent authors, venues, or arxiv ids. If unknown, omit the field.
- Don't pick more than 3 topics — over-tagging defeats the index.
- Don't `git commit` manually inside the skill — the Stop hook handles it.
