---
title: "LoRA-One: One-Step Full Gradient Could Suffice for Fine-Tuning Large Language Models, Provably and Efficiently"
url: https://arxiv.org/abs/2502.01235
type: paper
authors: [Yuanhe Zhang, Fanghui Liu, Yudong Chen]
venue: ICML 2025
year: 2025
topics: [theory, nlp]
added: 2026-05-14
arxiv_id: 2502.01235
---

# LoRA-One: One-Step Full Gradient Could Suffice for Fine-Tuning Large Language Models, Provably and Efficiently

**Link:** https://arxiv.org/abs/2502.01235

## Summary

This ICML 2025 oral paper provides a theoretical proof that LoRA adapters, under gradient descent, align with specific singular subspaces of the one-step full fine-tuning gradient. This result reveals the fundamental geometric structure of LoRA optimization: the adapter matrices converge to directions determined by the dominant singular vectors of the gradient at initialization, not arbitrary directions. The proposed method LoRA-One exploits this by initializing adapters directly from the one-step gradient, achieving immediate subspace alignment and provably linear convergence.

The theoretical analysis also shows how preconditioners can mitigate ill-conditioning in the LoRA optimization problem. By proving the adapter-to-gradient subspace alignment theorem, the paper explains both why LoRA works well (it implicitly finds the gradient's dominant singular directions) and why it can fail (if those directions are rank-degenerate, the LoRA rank collapses).

## Key points

- Proves LoRA adapters align to the singular subspaces of the one-step full fine-tuning gradient under gradient descent — a formal explanation of what LoRA actually learns.
- LoRA-One initializes from the one-step gradient for immediate subspace alignment; achieves linear convergence and improved generalization over standard LoRA.
- Preconditioners can theoretically mitigate ill-conditioning in LoRA's matrix-factorization objective.
- ICML 2025 oral — high authority theoretical contribution.
- Directly relevant to rank collapse: if the full-gradient's dominant singular subspace has low effective rank (e.g., under sparse RL rewards), LoRA's adapters collapse to that low-rank space.

## See also
- [[lora-convergence-implicit-bias]] — complementary landscape analysis (generic regime)
- [[lora-ntk-no-spurious-minima]] — NTK regime analysis
