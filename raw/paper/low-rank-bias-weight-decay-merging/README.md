---
title: "Low-rank bias, weight decay, and model merging in neural networks"
url: https://arxiv.org/abs/2502.17340
type: paper
authors: [Ilja Kuzborskij, Yasin Abbasi Yadkori]
year: 2025
topics: [theory, ml]
added: 2026-05-14
arxiv_id: 2502.17340
---

# Low-rank bias, weight decay, and model merging in neural networks

**Link:** https://arxiv.org/abs/2502.17340

## Summary

This paper formally characterizes the low-rank structural bias induced by L2 regularization (weight decay) at stationary points of gradient descent / gradient flow. The analysis covers shallow ReLU networks (gradient descent) and deep linear networks (gradient flow), proving that weight decay produces three linked properties at stationary points: (1) parameter-gradient alignment, (2) norm preservation across layers, and (3) systematic low-rank bias in weight matrices. These are not empirical observations but provable geometric consequences of the L2 penalty.

A second contribution connects this low-rank bias to model merging: two networks trained on approximately orthogonal input distributions can be merged by simple weight summation, with provable multitask performance guarantees. This is because weight decay constrains both models to low-rank solutions whose signal directions do not interfere.

## Key points

- Formally proves that L2 regularization at stationary points produces: parameter-gradient alignment, cross-layer norm preservation, and low-rank bias in weight matrices.
- Analysis covers shallow ReLU nets (GD) and deep linear nets (gradient flow) — goes beyond toy linear models.
- Low-rank structure is the mechanism enabling model merging via weight summation under orthogonal input distributions.
- Provides a unifying theoretical explanation for why weight decay routinely produces low-rank or near-low-rank solutions, complementing neural collapse literature.
- Relevant to LoRA rank collapse: weight decay in LoRA training provably drives adapter matrices toward low-rank stationary points, as shown here in a general setting.

## See also
- [[neural-collapse-low-rank-bias]] — companion result linking weight decay to neural collapse + low-rank bias
- [[lora-convergence-implicit-bias]] — shows zero-init + weight decay drive LoRA to low-rank global min
