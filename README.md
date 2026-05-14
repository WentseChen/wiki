# Wiki

Personal LLM-maintained knowledge base. Source links + LLM-compiled articles + derived outputs. Tiny, syncable, link-only.

## Layout

```
raw/        SOURCE MATERIAL — link-only stubs. One folder per blog/paper/project, README.md = the raw file.
articles/   COMPILED WIKI — LLM-maintained topics/, concepts/, summaries/, index.md.
outputs/    DERIVED — Q&A renders, Marp slides, matplotlib images, scratch notes.
```

LLM owns writes. You read in Obsidian (`~/wiki` as a vault). `[[slug]]` links resolve across `raw/`, `articles/concepts/`, `articles/summaries/`.

## Ingest a new entry

`/wiki-ingest <url>` — fetches, classifies, drops a raw stub, updates compiled wiki + index.

URL is mandatory. Blog/paper/project type is auto-detected (`arxiv.org/abs/*` → paper, `github.com/<org>/<repo>` → project, else blog).

## Bulk discovery by topic

`paper-search` subagent — fuzzy topic in, filtered + ingested entries out. Expands queries, searches arXiv / WebSearch / GitHub, filters for recent + high-impact, calls `/wiki-ingest` on each kept hit. Invoke via `Agent({ subagent_type: "paper-search", prompt: "<topic>" })` or natural-language ("find papers on X"). Defined at `.claude/agents/paper-search.md`.

## Topics (13)

`nlp · rl · agents · self-play · game-theory · multimodal · vision · systems · continuous-learning · theory · bandit · ml · others`

## Sync

`Stop` hook in `.claude/settings.json` auto commits + pushes to `origin/main` at the end of every Claude turn. Manual: `git add -A && git commit -m 'msg' && git push`.
