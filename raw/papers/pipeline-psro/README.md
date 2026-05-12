---
title: "Pipeline PSRO: A Scalable Approach for Finding Approximate Nash Equilibria in Large Games"
url: https://arxiv.org/abs/2006.08555
type: paper
authors: [Stephen McAleer, John Lanier, Roy Fox, Pierre Baldi]
venue: NeurIPS
year: 2020
topics: [rl, game-theory, agents]
added: 2026-05-11
arxiv_id: 2006.08555
---

# Pipeline PSRO: A Scalable Approach for Finding Approximate Nash Equilibria in Large Games

**Link:** https://arxiv.org/abs/2006.08555

## Summary
Parallelizes PSRO via a hierarchical pipeline: multiple RL workers train concurrently, each best-responding to the meta-Nash of the levels below; once the lowest active policy plateaus it becomes fixed and a new worker joins the top. Preserves PSRO's convergence guarantees while scaling linearly with parallel workers, and achieves state-of-the-art on Barrage Stratego, beating every existing bot.

## Key points
- First scalable parallel PSRO with convergence guarantees.
- Hierarchical pipeline of RL workers, lowest plays vs meta-Nash of fixed below.
- Avoids the divergence issues of DCH and Rectified PSRO in small games.
- SOTA on Barrage Stratego; large imperfect-info two-player zero-sum games.
- Open-sourced as `JBLanier/pipeline-psro`.

## See also
- [[unified-game-theoretic-marl]]
- [[xdo-extensive-form-double-oracle]]
