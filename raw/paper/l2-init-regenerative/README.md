---
title: Maintaining Plasticity in Continual Learning via Regenerative Regularization (L2 Init)
url: https://arxiv.org/abs/2308.11958
type: paper
authors: [Saurabh Kumar, Henrik Marklund, Benjamin Van Roy]
venue: CoLLAs 2025
year: 2023
topics: [continuous-learning, ml]
added: 2026-05-12
arxiv_id: 2308.11958
---

# Maintaining Plasticity in Continual Learning via Regenerative Regularization (L2 Init)

**Link:** https://arxiv.org/abs/2308.11958

## Summary
Kumar, Marklund, and Van Roy propose L2 Init: replace the standard L2 weight-decay term with one that pulls parameters toward their initial values. The motivation is identical to neuron-reset methods (parameters that are no longer useful should drift back to initialization, where they are most able to adapt), but the implementation is just a different penalty term.

Empirically, L2 Init beats EWC, MAS, shrink-and-perturb, and continual backprop on several Dohare-style continual supervised benchmarks. It's the cleanest "regularize, don't reset" alternative to continual backpropagation.

## Key points
- Single new hyperparameter; no architectural change.
- Outperforms several reset/regularize baselines on Dohare-style continual supervised tasks.
- Connects soft-reset, weight-decay, and re-init perspectives.
- Published version at CoLLAs 2025.

## See also
<!-- [[plasticity]] · [[warm-starting-shrink-perturb]] · [[capacity-loss-rl]] -->
