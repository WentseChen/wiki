---
title: Grandmaster Level in StarCraft II Using Multi-Agent Reinforcement Learning
url: https://www.nature.com/articles/s41586-019-1724-z
type: paper
authors: [Oriol Vinyals, Igor Babuschkin, Wojciech M. Czarnecki, et al.]
venue: Nature
year: 2019
topics: [rl, agents, self-play]
added: 2026-05-12
---

# AlphaStar: Grandmaster Level in StarCraft II

**Link:** https://www.nature.com/articles/s41586-019-1724-z

## Summary

AlphaStar reached Grandmaster rank across all three StarCraft II races on Battle.net under human-equivalent interface constraints. The system combines imitation learning from human replays, off-policy actor-critic RL, and a league-training scheme where main agents, main exploiters, and league exploiters interact to surface and patch strategic weaknesses, preventing strategy collapse typical of plain self-play.

## Key points
- Imitation pretrain on human replays bootstraps to top-15% before any self-play.
- League training: main agents + exploiter agents avoid cyclic forgetting of self-play.
- Fictitious-self-play style sampling over historical league snapshots.
- One unified neural net per race, latent variable conditions strategic openings — built-in strategy diversity.
- RSPO's StarCraft II evaluation domain.

## See also
- [[reward-switching-policy-optimization]]
- [[neural-fictitious-self-play]]
