---
title: "Beyond Perplexity: A Geometric and Spectral Study of Low-Rank Pre-Training"
url: https://arxiv.org/abs/2605.13652
type: paper
authors: [Namrata Shivagunde, Vijeta Deshpande, Sherin Muckatira, Anna Rumshisky]
year: 2026
topics: [ml, theory]
added: 2026-05-14
arxiv_id: "2605.13652"
---

# Beyond Perplexity: A Geometric and Spectral Study of Low-Rank Pre-Training

**Link:** https://arxiv.org/abs/2605.13652

## Summary

This paper investigates whether low-rank pre-training methods (GaLore, Fira, CoLA, SLTrain, ReLoRA) produce models that generalize comparably to full-rank training, using 16 evaluation metrics across loss landscape geometry, linear interpolation, spectral structure of weights, and activation similarity. Evaluated at scales from 60M to 350M parameters, the finding is clear: low-rank methods are not equivalent to full-rank training and converge to geometrically distinct solutions, even when perplexity scores are matched.

The spectral analysis dimension — examining singular value structure of weight matrices and learned updates — is directly relevant to the LoRA+RL intersection: it shows that matched perplexity does not imply matched weight geometry, which means spectral probes (effective rank, singular value distributions) reveal real differences between low-rank and full-rank adaptation that performance metrics miss. While the paper focuses on pre-training (not fine-tuning or RL), its methodology and findings apply directly to understanding why LoRA weight geometry differs from full fine-tuning even when benchmark scores seem comparable.

## Key points

- Low-rank pre-training methods converge to geometrically distinct solutions from full-rank training, despite matching perplexity.
- 16 evaluation metrics: loss landscape curvature, linear interpolation, spectral weight structure, activation similarity.
- Spectral structure of weights and updates reveals geometric differences invisible to perplexity metrics.
- Applies to GaLore, Fira, CoLA, SLTrain, ReLoRA across 60M–350M parameter scales.
- Methodological contribution: framework for evaluating low-rank solutions beyond task performance.

## See also
<!-- [[lora-vs-full-finetuning-illusion]] [[lora-spectral-geometry-training-objective]] [[rl-vs-sft-singular-vector-analysis]] -->
