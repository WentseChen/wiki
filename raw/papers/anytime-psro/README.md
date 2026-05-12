---
title: Anytime PSRO for Two-Player Zero-Sum Games
url: https://arxiv.org/abs/2201.07700
type: paper
authors: [Stephen McAleer, Kevin Wang, John Lanier, Marc Lanctot, Pierre Baldi, Tuomas Sandholm, Roy Fox]
venue: arXiv
year: 2022
topics: [rl, game-theory, agents]
added: 2026-05-11
arxiv_id: 2201.07700
---

# Anytime PSRO for Two-Player Zero-Sum Games

**Link:** https://arxiv.org/abs/2201.07700

## Summary
Standard double oracle / PSRO can see exploitability *increase* between iterations because the meta-distribution is restricted to the current strategy set. Anytime Double Oracle (ADO) instead picks the meta-distribution that minimizes exploitability against any policy in the *full* unrestricted game, guaranteeing monotone exploitability decrease and Nash convergence. APSRO is the deep-RL version using best-response RL.

## Key points
- ADO: meta-distribution minimizes exploitability vs full game, not restricted game.
- Monotone (anytime) exploitability reduction — no regressions.
- RM-BR DO: no-regret update against best responses to find the distribution.
- APSRO: deep-RL implementation of ADO.
- Lower final exploitability than DO and PSRO on Leduc + random normal-form games.

## See also
- [[unified-game-theoretic-marl]]
- [[pipeline-psro]]
- [[xdo-extensive-form-double-oracle]]
