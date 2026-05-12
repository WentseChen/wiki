---
title: Understanding and Preventing Capacity Loss in Reinforcement Learning
url: https://arxiv.org/abs/2204.09560
type: paper
authors: [Clare Lyle, Mark Rowland, Will Dabney]
venue: ICLR 2022
year: 2022
topics: [rl, theory, continuous-learning]
added: 2026-05-12
arxiv_id: 2204.09560
---

# Understanding and Preventing Capacity Loss in Reinforcement Learning

**Link:** https://arxiv.org/abs/2204.09560

## Summary
Lyle, Rowland, and Dabney formalize "capacity loss" as the inability of a trained network to fit new targets, and tie it to a measurable drop in feature rank that occurs as TD bootstraps non-stationary targets. Their InFeR regularizer maintains a subspace of features near their initial values, recovering performance especially on sparse-reward Atari.

This paper is one of the first to give the Dohare-style phenomenon a clean operational diagnostic (feature rank) and a non-reset-based fix (init-regularization rather than re-init). It complements Dohare by suggesting "stay near init" as an alternative to "selectively re-init."

## Key points
- Defines capacity loss; quantifies it via feature rank.
- Shows it is triggered by non-stationary target sequences, not just RL specifically.
- Introduces InFeR: regress a feature subspace toward initialization.
- Spotlight at ICLR 22; one of the earliest plasticity-flavored RL diagnoses.

## See also
<!-- [[plasticity]] · [[l2-init-regenerative]] · [[implicit-under-parameterization]] -->
