---
title: On Warm-Starting Neural Network Training
url: https://arxiv.org/abs/1910.08475
type: paper
authors: [Jordan T. Ash, Ryan P. Adams]
venue: NeurIPS 2020
year: 2020
topics: [ml, continuous-learning]
added: 2026-05-12
arxiv_id: 1910.08475
---

# On Warm-Starting Neural Network Training

**Link:** https://arxiv.org/abs/1910.08475

## Summary
Ash and Adams document the surprising fact that adding new training data to a converged network and continuing training produces worse generalization than re-training from random init. Their shrink-and-perturb fix multiplies weights by a constant < 1 then adds small noise, recovering from-scratch performance while keeping warm-start's speed advantage.

This is the seminal supervised-learning paper that establishes "trained nets are harder to train further" as a real, isolated phenomenon — separate from catastrophic forgetting. Dohare's continual backprop generalizes the shrink-and-perturb idea from a one-shot whole-net operation to a per-unit, every-step operation guided by utility.

## Key points
- Demonstrates the warm-start generalization gap on CIFAR/ImageNet.
- Shrink-and-perturb: w := lambda*w + epsilon*noise, with lambda~0.4.
- First popularization of "reset to recover" outside RL.
- Influential template for plasticity-restoration interventions.

## See also
<!-- [[plasticity]] · [[l2-init-regenerative]] -->
