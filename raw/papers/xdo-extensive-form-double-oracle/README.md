---
title: "XDO: A Double Oracle Algorithm for Extensive-Form Games"
url: https://arxiv.org/abs/2103.06426
type: paper
authors: [Stephen McAleer, John Lanier, Kevin Wang, Pierre Baldi, Roy Fox]
venue: NeurIPS
year: 2021
topics: [rl, game-theory, agents]
added: 2026-05-11
arxiv_id: 2103.06426
---

# XDO: A Double Oracle Algorithm for Extensive-Form Games

**Link:** https://arxiv.org/abs/2103.06426

## Summary
PSRO mixes policies only at the root, so on sequential games it may need exponentially many iterations in the number of infostates. XDO instead mixes best responses at every infostate of the extensive-form game, guaranteeing linear convergence in infostate count. Neural XDO (NXDO) learns the best response with deep RL — the first deep RL method to find an approximate Nash in high-dimensional continuous-action sequential games.

## Key points
- Mixes policies at every infostate, not just the root.
- Linear-in-infostates convergence (vs PSRO's exponential worst case).
- Tabular XDO matches/beats CFR on Leduc poker / Oshi-Zumo.
- NXDO: first deep-RL Nash solver for continuous-action sequential games.
- Order-of-magnitude fewer iterations than PSRO on Leduc.

## See also
- [[pipeline-psro]]
- [[unified-game-theoretic-marl]]
