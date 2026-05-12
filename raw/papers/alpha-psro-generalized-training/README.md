---
title: A Generalized Training Approach for Multiagent Learning
url: https://arxiv.org/abs/1909.12823
type: paper
authors: [Paul Muller, Shayegan Omidshafiei, Mark Rowland, Karl Tuyls, Julien Perolat, Siqi Liu, Daniel Hennes, Luke Marris, Marc Lanctot, Edward Hughes, Zhe Wang, Guy Lever, Nicolas Heess, Thore Graepel, Remi Munos]
venue: ICLR
year: 2020
topics: [rl, game-theory, agents]
added: 2026-05-11
arxiv_id: 1909.12823
---

# A Generalized Training Approach for Multiagent Learning

**Link:** https://arxiv.org/abs/1909.12823

## Summary
Generalizes PSRO from two-player zero-sum to general-sum, many-player games by swapping the Nash meta-solver for α-Rank — yielding α-PSRO. The α-Rank meta-solver is unique (no equilibrium-selection issues) and polynomial-time, sidestepping Nash intractability. Demonstrates faster convergence than Nash-based PSRO on 3–5-player Kuhn and Leduc poker.

## Key points
- Introduces α-PSRO: PSRO with α-Rank as meta-solver.
- Removes the two-player zero-sum restriction of vanilla PSRO.
- Unique meta-distribution → no equilibrium-selection ambiguity.
- Outperforms Nash-based PSRO on many-player Kuhn/Leduc poker.
- Establishes α-Rank as a principled tool for population-based MARL.

## See also
- [[alpha-rank]]
- [[unified-game-theoretic-marl]]
