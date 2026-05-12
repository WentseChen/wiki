---
title: Overcoming Catastrophic Forgetting in Neural Networks (EWC)
url: https://arxiv.org/abs/1612.00796
type: paper
authors: [James Kirkpatrick, Razvan Pascanu, Neil Rabinowitz, Joel Veness, Guillaume Desjardins, Andrei A. Rusu, Kieran Milan, John Quan, Tiago Ramalho, Agnieszka Grabska-Barwinska, Demis Hassabis, Claudia Clopath, Dharshan Kumaran, Raia Hadsell]
venue: PNAS
year: 2017
topics: [continuous-learning, theory]
added: 2026-05-12
arxiv_id: 1612.00796
---

# Overcoming Catastrophic Forgetting in Neural Networks (EWC)

**Link:** https://arxiv.org/abs/1612.00796

## Summary
Kirkpatrick et al. introduce Elastic Weight Consolidation, the canonical regularization-based continual-learning method: after training task k, anchor the network with a quadratic penalty toward the converged weights, scaled by the diagonal Fisher (importance) of each parameter. They demonstrate it on permuted MNIST and sequential Atari.

Included here as the canonical catastrophic-forgetting reference. Although CF is distinct from plasticity loss (in fact often the opposite trade-off — protecting old weights reduces plasticity), every plasticity paper grounds itself against EWC, and the Dohare Nature paper explicitly distinguishes the two phenomena. EWC also pioneered the "importance score per parameter" idea that Dohare's utility score echoes.

## Key points
- Seminal Bayesian-motivated penalty for sequential task learning.
- Diagonal Fisher importance as a proxy for synaptic consolidation.
- Inspired SI, MAS, and the broader regularization-based CL family.
- High-citation count (~10k+); essential grounding reference.

## See also
<!-- [[plasticity]] · [[l2-init-regenerative]] -->
