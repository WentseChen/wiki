---
title: Implicit Under-Parameterization Inhibits Data-Efficient Deep Reinforcement Learning
url: https://arxiv.org/abs/2010.14498
type: paper
authors: [Aviral Kumar, Rishabh Agarwal, Dibya Ghosh, Sergey Levine]
venue: ICLR 2021
year: 2021
topics: [rl, theory]
added: 2026-05-12
arxiv_id: 2010.14498
---

# Implicit Under-Parameterization Inhibits Data-Efficient Deep Reinforcement Learning

**Link:** https://arxiv.org/abs/2010.14498

## Summary
Kumar et al. show that iterated regression onto self-generated targets — the heart of TD with neural nets — drives the feature matrix of the value network toward low effective rank. They both characterize this empirically across Atari/Gym and prove it for a linearized analysis, identifying it as a pathological interaction between bootstrapping and gradient descent.

This is the foundational rank-collapse paper that the plasticity-loss literature retroactively connects to. Dohare and Abbas both cite under-parameterization as one of several aliases for what they call loss of plasticity.

## Key points
- Identifies effective-rank collapse in deep value networks.
- Distinct from capacity loss in framing (rank as expressivity vs. trainability), but tightly related.
- Formal analysis in linearized regime; empirics across offline + online Atari.
- Predates and predicts much of the plasticity-loss empirical agenda.

## See also
<!-- [[plasticity]] · [[capacity-loss-rl]] -->
