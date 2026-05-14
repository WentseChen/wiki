---
title: "LoRA Training in the NTK Regime has No Spurious Local Minima"
url: https://arxiv.org/abs/2402.11867
type: paper
authors: [Uijeong Jang, Jason D. Lee, Ernest K. Ryu]
venue: ICML 2024
year: 2024
topics: [theory, ml]
added: 2026-05-14
arxiv_id: 2402.11867
---

# LoRA Training in the NTK Regime has No Spurious Local Minima

**Link:** https://arxiv.org/abs/2402.11867

## Summary

This paper provides formal theoretical guarantees for LoRA fine-tuning in the Neural Tangent Kernel (NTK) regime. The key result is that full fine-tuning admits a low-rank solution of rank r ≲ √N, and that using LoRA with rank r ≳ √N eliminates all spurious local minima from the optimization landscape, allowing gradient descent to reliably find these low-rank solutions. The work gives a principled rank threshold — tied to dataset size — above which LoRA's constrained optimization is globally well-behaved.

## Key points

- Full fine-tuning objective has low-rank global solutions with rank scaling as √N (N = number of data points).
- LoRA with rank ≳ √N has no spurious local minima in the NTK regime; gradient descent converges to a global optimum.
- Solutions found via LoRA generalize effectively despite constrained parameterization.
- The rank threshold √N provides a concrete, data-size-dependent prescription for choosing LoRA rank.
- Analysis is in the NTK (lazy training / linearization) regime — the complementary generic-regime analysis appears in Kim et al. 2025 [[lora-convergence-implicit-bias]].

## See also
- [[lora-convergence-implicit-bias]] — generic-regime complement to this NTK analysis
