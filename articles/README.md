# articles/ — compiled wiki

LLM-maintained. Don't hand-edit unless you mean to.

## Subfolders

- `index.md` — master entry. Links to every topic + a rolling "Recent additions" list (cap 20).
- `topics/<topic>.md` — one per topic. Sections: `## Overview`, `## Key concepts`, `## Recent`.
- `concepts/<concept>.md` — one per specific concept (e.g. `ppo.md`, `mcts.md`). Sections: short definition + `## Sources` (links back to raw entries).
- `summaries/<slug>.md` — 1-paragraph summary per raw entry. Used for fast retrieval / search.

## Links

Use `[[slug]]` for Obsidian wiki-links. They resolve across `raw/<type>/<slug>/`, `concepts/<slug>.md`, and `summaries/<slug>.md` as long as basenames are unique.

## Maintenance

- `/wiki-ingest <url>` updates this whole tree atomically when a new entry lands.
- Periodic lints / Q&A passes may refine topic overviews and concept stubs over time.
