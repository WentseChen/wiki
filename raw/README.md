# raw/ — source material

One folder per entry: `raw/<type>/<slug>/`. Types: `blogs`, `papers`, `projects`.

The folder's `README.md` IS the raw file — frontmatter + URL + summary. `notes.md` and `images/` are optional, added on demand.

## Slug rules

- kebab-case from the title, ≤6 words
- collision-safe: if `<slug>` exists, append `-2`, `-3`, …

## Entry template

```markdown
---
title: <title>
url: <url>                     # MANDATORY
type: blog | paper | project
authors: [name1, name2]
venue: <conf/journal/org>      # optional
year: 2026
topics: [rl, self-play]        # 1–3 from the 13-topic list
added: YYYY-MM-DD
arxiv_id: 2405.12345           # papers only, optional
github: org/repo               # projects only, optional
---

# <title>

**Link:** <url>

## Summary
<1–3 paragraphs — what it is, key claim, why it's interesting>

## Key points
- ...

## See also
- [[<slug-of-related-entry>]]
```

## Adding entries

Use `/wiki-ingest <url>`. It writes the raw entry AND updates `articles/` (topics, concepts, summaries, index) in one pass.
