---
title: Loss of Plasticity in Continual Deep Reinforcement Learning
url: https://arxiv.org/abs/2303.07507
type: paper
authors: [Zaheer Abbas, Rosie Zhao, Joseph Modayil, Adam White, Marlos C. Machado]
venue: CoLLAs 2023
year: 2023
topics: [rl, continuous-learning]
added: 2026-05-12
arxiv_id: 2303.07507
---

# Loss of Plasticity in Continual Deep Reinforcement Learning

**Link:** https://arxiv.org/abs/2303.07507

## Summary
Abbas et al. build a continual-Atari benchmark in which value-based agents cycle through several games for billions of frames, and show convincingly that the agents progressively lose the ability to make progress on new games, even at sequences spanning 50 days of training. They trace the failure to weight-norm explosion and dead units, and show that CReLU activations (which double the channel, keeping both positive and negative parts) drastically reduce dying units and recover plasticity.

This is the canonical continual-RL plasticity-loss paper and the direct sibling of Dohare's RL experiments. It provides the architectural-side fix (CReLU) that complements Dohare's algorithmic-side fix (continual backprop).

## Key points
- Multi-game continual Atari benchmark at very large scale (2B frames, 50 days).
- Cleanly attributes plasticity loss to weight norm growth + dead ReLUs.
- CReLU as a simple, drop-in mitigation.
- One of the seminal "plasticity loss in RL" papers cited by Dohare.

## See also
<!-- [[plasticity]] · [[dormant-neuron-phenomenon]] · [[primacy-bias-deep-rl]] -->
