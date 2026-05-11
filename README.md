# Wiki

Personal research wiki. Link-based — no PDFs/HTML stored locally, only URLs + short notes. Keeps the repo tiny.

## Layout

```
papers/    research papers           (arxiv, conf proceedings, ...)
blogs/     research / engineering blogs
projects/  open-source projects + repos
```

Each type splits into 13 topic folders:

`nlp` · `rl` · `agents` · `self-play` · `game-theory` · `multimodal` · `vision` · `systems` · `continuous-learning` · `theory` · `bandit` · `ml` · `others`

## Add an entry

Pick the right `<type>/<topic>/README.md` and prepend (newest at top):

```markdown
- [Title](https://...) — one-line note. *Authors, venue/year.* `arxiv:1234.5678`
```

Drop the citation/id parts you don't have. Keep the note short — the link does the rest.

Unsure of topic? Use `others/`.

## Sync

Stop hook in `.claude/settings.json` auto commits + pushes to `origin/main` at the end of every Claude turn. To sync manually: `git add -A && git commit -m 'msg' && git push`.
