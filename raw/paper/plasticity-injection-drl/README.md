---
title: Deep Reinforcement Learning with Plasticity Injection
url: https://arxiv.org/abs/2305.15555
type: paper
authors: [Evgenii Nikishin, Junhyuk Oh, Georg Ostrovski, Clare Lyle, Razvan Pascanu, Will Dabney, Andre Barreto]
venue: NeurIPS 2023
year: 2023
topics: [rl, continuous-learning]
added: 2026-05-12
arxiv_id: 2305.15555
---

# Deep Reinforcement Learning with Plasticity Injection

**Link:** https://arxiv.org/abs/2305.15555

## Summary
Nikishin et al. propose plasticity injection: replace some hidden layer with f(x) = old_f(x) + (g(x) - g_frozen(x)) where g is a fresh copy of f; this leaves predictions unchanged at injection time but adds new trainable capacity. The procedure cleanly tests whether a stalled agent is stalled due to lost plasticity (injection helps) vs. data limits (injection doesn't), and also serves as a training-time intervention.

Included for diversity of angle: it's neither a reset nor a regularizer, but a network-growth method, and it doubles as a diagnostic tool — exactly the kind of mechanism-isolating experiment Dohare's Nature paper benefits from being compared against.

## Key points
- Zero-impact injection: prediction unchanged at injection step.
- Doubles as a causal probe for "is plasticity the bottleneck here?"
- Compatible with dynamic network growth.
- NeurIPS 2023 spotlight.

## See also
<!-- [[plasticity]] · [[primacy-bias-deep-rl]] · [[dormant-neuron-phenomenon]] -->
