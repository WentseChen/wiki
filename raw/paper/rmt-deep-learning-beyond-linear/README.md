---
title: "Random Matrix Theory for Deep Learning: Beyond Eigenvalues of Linear Models"
url: https://arxiv.org/abs/2506.13139
type: paper
authors: [Zhenyu Liao, Michael W. Mahoney]
venue: IEEE Signal Processing Magazine
year: 2025
topics: [theory, ml]
added: 2026-05-14
arxiv_id: 2506.13139
---

# Random Matrix Theory for Deep Learning: Beyond Eigenvalues of Linear Models

**Link:** https://arxiv.org/abs/2506.13139

## Summary

This journal paper (IEEE Signal Processing Magazine) extends classical Random Matrix Theory to the full setting of deep, nonlinear neural networks trained in high-dimensional overparameterized regimes. Classical RMT analyzed eigenvalue distributions of random linear models; this work goes further by introducing the "High-dimensional Equivalent" framework that systematically handles three challenges classical tools cannot: high dimensionality, nonlinearity, and analysis of generic eigenspectral functionals (not just the distribution of eigenvalues).

The framework recovers known phenomena — scaling laws, double descent, sample-wise and model-wise phase transitions — and provides precise theoretical characterizations of training and generalization across linear models, shallow networks, and deep architectures. This is the theoretical backbone for using spectral tools (singular value spectra, effective rank) to understand fine-tuning dynamics, including RL-induced rank collapse.

## Key points

- Introduces the "High-dimensional Equivalent" as a unified generalization of Deterministic and Linear Equivalents for handling nonlinear deep networks at scale.
- Extends RMT to analyze training and generalization precisely across linear, shallow, and deep architectures in the proportional (n ≈ d ≈ p) regime.
- Captures scaling laws, double descent, and nonlinear learning dynamics under a single theoretical umbrella.
- Published in IEEE Signal Processing Magazine — a high-authority journal venue.
- Provides the rigorous spectral foundation for using singular-value / effective-rank metrics to analyze rank collapse in fine-tuned LLMs.

## See also
- [[rmt-transformer-singular-values]] — empirical RMT analysis of transformer singular-value spectra
