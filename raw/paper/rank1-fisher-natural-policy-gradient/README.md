---
title: "Rank-1 Approximation of Inverse Fisher for Natural Policy Gradients in Deep Reinforcement Learning"
url: https://arxiv.org/abs/2601.18626
type: paper
authors: [Yingxiao Huo, Satya Prakash Dash, Radu Stoican, Samuel Kaski, Mingfei Sun]
year: 2026
topics: [rl, theory]
added: 2026-05-14
arxiv_id: 2601.18626
---

# Rank-1 Approximation of Inverse Fisher for Natural Policy Gradients in Deep Reinforcement Learning

**Link:** https://arxiv.org/abs/2601.18626

## Summary

This paper addresses the computational bottleneck of inverting the Fisher Information Matrix (FIM) in natural policy gradient methods for deep RL. The authors propose a rank-1 approximation to the inverse-FIM, which reduces the inversion cost from O(n²) to O(n) per step while preserving the covariant geometry of natural gradient updates. The key theoretical result is that under certain conditions, the rank-1 approximation converges faster than standard policy gradients and achieves sample complexity comparable to stochastic policy gradient methods.

The FIM-rank angle is directly relevant to the rank-collapse problem: the FIM of a policy summarizes the geometry of the policy's update directions, and if RL training induces a low-rank FIM (as expected under sparse or high-variance rewards, where the policy's information geometry is degenerate), natural gradient methods naturally collapse to low-rank updates — a formal geometric argument for why reward sparsity induces rank-degenerate parameter updates.

## Key points

- Rank-1 approximation to the inverse-FIM enables scalable natural policy optimization for deep RL.
- Formally proves: under stated conditions, rank-1 FIM approximation converges faster than vanilla policy gradients and matches stochastic PG sample complexity.
- Low-rank FIM geometry is the mechanistic link between sparse/high-variance RL rewards and degenerate (low-rank) gradient updates — relevant to LoRA rank collapse.
- Empirically outperforms standard actor-critic and trust-region baselines.
- Fresh preprint (Jan 2026), not yet published at a conference.

## See also
- [[lora-one-singular-subspace]] — singular subspace alignment view of LoRA updates
- [[lora-convergence-implicit-bias]] — implicit bias toward low-rank in LoRA training
