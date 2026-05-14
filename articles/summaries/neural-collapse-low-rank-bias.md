# Provable Emergence of Deep Neural Collapse and Low-Rank Bias in L²-Regularized Nonlinear Networks

*paper, 2024. Emanuele Zangrando et al.*

Proves that L² weight decay jointly drives two phenomena: Deep Neural Collapse (within-class feature clusters collapse to a point) and low-rank bias in weight matrices. The key bound shows distance to rank-K is proportional to Total Cluster Variation / λ, so the same weight-decay parameter that causes neural collapse forces weight matrices toward low rank — directly motivating why LoRA training with weight decay produces rank-degenerate updates.

→ [raw entry](../../raw/paper/neural-collapse-low-rank-bias/README.md) · [url](https://arxiv.org/abs/2402.03991)
