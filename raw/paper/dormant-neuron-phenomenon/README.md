---
title: The Dormant Neuron Phenomenon in Deep Reinforcement Learning
url: https://arxiv.org/abs/2302.12902
type: paper
authors: [Ghada Sokar, Rishabh Agarwal, Pablo Samuel Castro, Utku Evci]
venue: ICML 2023
year: 2023
topics: [rl, continuous-learning]
added: 2026-05-12
arxiv_id: 2302.12902
---

# The Dormant Neuron Phenomenon in Deep Reinforcement Learning

**Link:** https://arxiv.org/abs/2302.12902

## Summary
Sokar et al. quantify dormancy via a normalized activation magnitude and show that the dormant fraction grows monotonically during DQN/Rainbow training, eating network capacity. Their ReDo method periodically checks for dormant units and reinitializes their incoming/outgoing weights, which cleanly halts the capacity bleed and boosts Atari performance.

This is the most mechanistically aligned RL-side paper to Dohare's continual-backprop: both diagnose the same micro-symptom (units going silent / low utility) and both prescribe per-unit reinitialization. Dohare extends the story to supervised learning, multi-billion-step continual settings, and replaces ReDo's activation-magnitude criterion with a utility-based one.

## Key points
- Defines a dormancy score; demonstrates monotonic increase across DQN, DrQ, SAC.
- ReDo: periodically re-init dormant units (both incoming and outgoing weights).
- Improves Atari and DM-Control across replay ratios.
- Bridges representation-collapse and plasticity-loss literatures.

## See also
<!-- [[plasticity]] · [[primacy-bias-deep-rl]] · [[plasticity-loss-continual-drl]] -->
