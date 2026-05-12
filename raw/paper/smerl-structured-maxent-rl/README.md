---
title: One Solution is Not All You Need - Few-Shot Extrapolation via Structured MaxEnt RL
url: https://arxiv.org/abs/2010.14484
type: paper
authors: [Saurabh Kumar, Aviral Kumar, Sergey Levine, Chelsea Finn]
venue: NeurIPS
year: 2020
topics: [rl]
added: 2026-05-12
arxiv_id: 2010.14484
---

# One Solution is Not All You Need (SMERL)

**Link:** https://arxiv.org/abs/2010.14484

## Summary

SMERL trains a single agent to find multiple near-optimal solutions to one MDP by augmenting max-entropy RL with a latent-conditioned diversity bonus, so each latent indexes a different way to solve the task. The authors characterize a robustness set — environments where the resulting policy set generalizes few-shot — showing that having multiple solutions yields zero-/few-shot extrapolation to perturbed dynamics.

## Key points
- Multiple near-optimal solutions in one training run, indexed by a latent.
- Few-shot extrapolation to test-time perturbations without training on those perturbations.
- Diversity bonus active only above a reward threshold — preserves task performance.
- Closest algorithmic sibling to RSPO in the diverse-near-optimal cluster.

## See also
- [[reward-switching-policy-optimization]]
- [[diverse-successor-features]]
- [[domino-diversity-near-optimality]]
