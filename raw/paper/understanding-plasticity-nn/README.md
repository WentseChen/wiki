---
title: Understanding Plasticity in Neural Networks
url: https://arxiv.org/abs/2303.01486
type: paper
authors: [Clare Lyle, Zeyu Zheng, Evgenii Nikishin, Bernardo Avila Pires, Razvan Pascanu, Will Dabney]
venue: ICML 2023
year: 2023
topics: [theory, rl, continuous-learning]
added: 2026-05-12
arxiv_id: 2303.01486
---

# Understanding Plasticity in Neural Networks

**Link:** https://arxiv.org/abs/2303.01486

## Summary
Lyle et al. systematically disentangle proposed causes of plasticity loss and demonstrate that the dominant signal is curvature, not unit saturation: networks lose plasticity even when no unit is dead, and Hessian eigenvalues blow up consistently. They identify design choices (layer norm, residual connections, careful parameterization, optimizer state) that preserve plasticity without explicit resets.

This is the most mechanistically incisive plasticity-loss paper and a useful counterpoint to Dohare. It suggests dead units are a symptom, not the root cause, and motivates a richer toolbox (norm + careful init + optimizer choice) for plasticity preservation.

## Key points
- Curvature is the dominant correlate of plasticity loss.
- Dead/saturated units are neither necessary nor sufficient.
- Layer normalization + careful init dramatically helps.
- Validates on Atari at scale.

## See also
<!-- [[plasticity]] · [[capacity-loss-rl]] · [[dormant-neuron-phenomenon]] -->
