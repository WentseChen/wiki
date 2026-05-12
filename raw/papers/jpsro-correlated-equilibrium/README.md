---
title: Multi-Agent Training beyond Zero-Sum with Correlated Equilibrium Meta-Solvers
url: https://arxiv.org/abs/2106.09435
type: paper
authors: [Luke Marris, Paul Muller, Marc Lanctot, Karl Tuyls, Thore Graepel]
venue: ICML
year: 2021
topics: [rl, game-theory, agents]
added: 2026-05-11
arxiv_id: 2106.09435
---

# Multi-Agent Training beyond Zero-Sum with Correlated Equilibrium Meta-Solvers

**Link:** https://arxiv.org/abs/2106.09435

## Summary
Extends PSRO to n-player, general-sum extensive-form games via Joint PSRO (JPSRO), which uses (coarse) correlated equilibrium meta-solvers instead of Nash. Introduces Maximum Gini Correlated Equilibrium (MGCE) — a tractable, principled selection rule from the convex CE polytope — and proves convergence to JPSRO-CCE or JPSRO-CE. CEs are tractable in n-player games, allow signaling/coordination, and yield higher social welfare than Nash.

## Key points
- JPSRO: PSRO with (C)CE meta-solvers for general-sum n-player games.
- MGCE: principled, computationally efficient correlated-equilibrium selection.
- Convergence guarantees beyond zero-sum.
- CE coordination → higher-value solutions than Nash in cooperative games.
- Unifies competitive and cooperative multi-agent training.

## See also
- [[unified-game-theoretic-marl]]
- [[alpha-psro-generalized-training]]
