---
title: "Small Singular Values Matter: A Random Matrix Analysis of Transformer Models"
url: https://arxiv.org/abs/2410.17770
type: paper
authors: [Max Staats, Matthias Thamm, Bernd Rosenow]
year: 2024
topics: [theory, nlp]
added: 2026-05-14
arxiv_id: 2410.17770
---

# Small Singular Values Matter: A Random Matrix Analysis of Transformer Models

**Link:** https://arxiv.org/abs/2410.17770

## Summary

This paper uses Random Matrix Theory (RMT) as a zero-information baseline — specifically, the Marchenko-Pastur distribution for randomly initialized weights — and identifies where the singular-value spectra of pretrained transformer weight matrices deviate from it. The key finding is that significant learned structure appears at *both* ends of the spectrum: not only among the largest singular values (as conventionally assumed) but also among the *smallest*. Removing the RMT-deviating singular values (at either extreme) substantially increases perplexity; removing only the bulk (RMT-consistent) values has minimal effect.

The work shows that singular vectors associated with small singular values have high overlap with the eigenvectors of the activation covariance matrices wherever RMT is violated, confirming they encode learned, task-relevant structure. After fine-tuning, the smallest decile of singular values becomes the third most influential spectrum component — directly relevant to understanding what happens to the singular value spectrum during RL fine-tuning (where effective rank collapse may shift information toward the extremes).

## Key points

- RMT (Marchenko-Pastur) serves as a zero-information hypothesis: deviations at both spectrum ends indicate learned structure.
- Small singular values carry significant information — their eigenvectors align with activation covariance eigenvectors wherever RMT is violated.
- Removing RMT-deviating singular values sharply increases perplexity; removing the bulk does not.
- After fine-tuning, the smallest decile of SVs is the third most influential component.
- Provides a principled RMT framework for analyzing rank collapse: shifts in the spectrum during RL fine-tuning can be detected as departures from the Marchenko-Pastur law.

## See also
- [[rmt-deep-learning-beyond-linear]] — broader RMT theory for nonlinear deep networks
- [[lora-spectral-geometry-training-objective]] — spectral analysis of LoRA deltas classifying training objective
