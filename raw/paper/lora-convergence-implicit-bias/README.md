---
title: "LoRA Training Provably Converges to a Low-Rank Global Minimum or It Fails Loudly (But it Probably Won't Fail)"
url: https://arxiv.org/abs/2502.09376
type: paper
authors: [Junsu Kim, Jaeyeon Kim, Ernest K. Ryu]
year: 2025
topics: [theory, ml]
added: 2026-05-14
arxiv_id: 2502.09376
---

# LoRA Training Provably Converges to a Low-Rank Global Minimum or It Fails Loudly (But it Probably Won't Fail)

**Link:** https://arxiv.org/abs/2502.09376

## Summary

This paper provides a rigorous theoretical analysis of LoRA's optimization landscape without relying on restrictive linearization assumptions. The central result is a convergence dichotomy: in the "generic regime" (the practical setting where linearization does not hold), LoRA training either converges to a global minimizer with low rank and small magnitude, or to a qualitatively distinct spurious local minimum with high rank and large magnitude. The authors attribute LoRA's empirical reliability to an implicit bias induced by zero-initialization and weight decay, which steers optimization toward the well-behaved low-rank region.

## Key points

- Distinguishes between "special regime" (linearization holds, NTK analysis applies) and "generic regime" (realistic, non-linear) for LoRA loss landscape analysis.
- Proves convergence dichotomy: low-rank global minimum or high-rank spurious local minimum — no in-between; the latter is rare in practice.
- Zero-initialization of adapter B and L2 weight decay together create an implicit bias toward the low-rank, small-magnitude basin.
- Extends prior theoretical work (which relied on linearization or toy setups) to the full non-convex optimization landscape.
- Directly relevant to rank collapse: explains why LoRA's rank does not expand freely under gradient descent — the implicit bias suppresses it.

## See also
<!-- [[lora-ntk-no-spurious-minima]] -->
<!-- [[lora-one-singular-subspace]] -->
