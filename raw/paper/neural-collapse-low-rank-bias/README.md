---
title: "Provable Emergence of Deep Neural Collapse and Low-Rank Bias in L²-Regularized Nonlinear Networks"
url: https://arxiv.org/abs/2402.03991
type: paper
authors: [Emanuele Zangrando, Piero Deidda, Simone Brugiapaglia, Nicola Guglielmi, Francesco Tudisco]
year: 2024
topics: [theory, ml]
added: 2026-05-14
arxiv_id: 2402.03991
---

# Provable Emergence of Deep Neural Collapse and Low-Rank Bias in L²-Regularized Nonlinear Networks

**Link:** https://arxiv.org/abs/2402.03991

## Summary

This paper establishes a rigorous theoretical connection between two phenomena that co-occur under L² (weight decay) regularization: Deep Neural Collapse (DNC1 — the convergence of within-class feature clusters to a point) and low-rank bias in weight matrices. The central result is a quantitative bound: the distance from a weight matrix to the set of rank-K matrices is bounded above by the Total Cluster Variation (TCV) of intermediate embeddings, scaled inversely by the weight-decay parameter. This shows that as weight decay drives TCV to zero (neural collapse), it simultaneously drives the weight matrices toward low rank — the two phenomena are "intimately linked" products of the same optimization geometry.

The paper also proves global optimality of DNC1 under a constrained representation-cost setting for both feedforward and residual architectures, and shows that a continuous loss-decreasing path from nearly any initialization to a globally optimal DNC1-satisfying configuration exists — implying a benign optimization landscape under L² regularization.

## Key points

- Distance to rank-K approximation is bounded by TCV/λ (λ = weight-decay strength): neural collapse and low-rank bias are jointly controlled by weight decay.
- Proves DNC1 is globally optimal under the representation-cost objective for feedforward and residual architectures.
- Continuous, loss-decreasing path exists from typical initializations to global optima — no bad local minima under weight decay.
- Unified framework: both neural collapse and low-rank bias emerge as geometric consequences of L² regularization, not separate phenomena.
- Directly relevant to rank collapse in fine-tuning: weight decay (used in LoRA training) provably biases weight matrices toward lower rank.

## See also
- [[lora-convergence-implicit-bias]] — shows weight decay induces implicit low-rank bias in LoRA specifically
