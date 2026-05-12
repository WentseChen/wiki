---
title: "NeuPL: Neural Population Learning"
url: https://arxiv.org/abs/2202.07415
type: paper
authors: [Siqi Liu, Luke Marris, Daniel Hennes, Josh Merel, Nicolas Heess, Thore Graepel]
venue: ICLR
year: 2022
topics: [rl, game-theory, agents]
added: 2026-05-11
arxiv_id: 2202.07415
---

# NeuPL: Neural Population Learning

**Link:** https://arxiv.org/abs/2202.07415

## Summary
Replaces PSRO's iterative "train, freeze, add" loop with a single conditional network that represents the entire population, where each policy is conditioned on a meta-game mixture. All policies train concurrently and continually, eliminating wasteful re-learning of basic skills and avoiding premature truncation of best responses. Supports cyclic interaction graphs beyond PSRO's scope, with convergence guarantees under mild assumptions.

## Key points
- One conditional network instead of a growing set of independent policies.
- Concurrent training of all policies — no freeze-and-add.
- Transfer learning across policies via shared representation.
- Handles cyclic interaction graphs (beyond PSRO).
- Improved sample/compute efficiency vs PSRO at scale.

## See also
- [[unified-game-theoretic-marl]]
- [[pipeline-psro]]
