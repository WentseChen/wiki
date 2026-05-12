---
title: Open-ended Learning in Symmetric Zero-sum Games
url: https://arxiv.org/abs/1901.08106
type: paper
authors: [David Balduzzi, Marta Garnelo, Yoram Bachrach, Wojciech Czarnecki, Julien Perolat, Max Jaderberg, Thore Graepel]
venue: ICML
year: 2019
topics: [rl, game-theory, self-play]
added: 2026-05-11
arxiv_id: 1901.08106
---

# Open-ended Learning in Symmetric Zero-sum Games

**Link:** https://arxiv.org/abs/1901.08106

## Summary
Introduces a geometric "gamescape" framework for nontransitive zero-sum games (rock-paper-scissors style cycles), where simple self-play and PSRO with Nash meta-solver leave gaps. Proposes Rectified Nash Response (PSRO_rN), which only trains new agents against opponents they beat — a niching mechanism that grows a diverse, broadly-effective population rather than chasing a single dominant strategy.

## Key points
- Frames population learning geometrically via a "gamescape" of payoffs.
- Diagnoses why naive self-play / PSRO fail in nontransitive games.
- Rectified Nash Response: niche-aware best-response training.
- Produces stronger, more diverse populations than vanilla PSRO.
- Foundational reference for diversity-based PSRO variants.

## See also
- [[unified-game-theoretic-marl]]
- [[diverse-psro-behavioural-diversity]]
