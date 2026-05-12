---
title: Effective Diversity in Population Based Reinforcement Learning
url: https://arxiv.org/abs/2002.00632
type: paper
authors: [Jack Parker-Holder, Aldo Pacchiano, Krzysztof Choromanski, Stephen Roberts]
venue: NeurIPS
year: 2020
topics: [rl]
added: 2026-05-12
arxiv_id: 2002.00632
---

# Effective Diversity in Population Based Reinforcement Learning (DvD)

**Link:** https://arxiv.org/abs/2002.00632

## Summary

DvD measures the diversity of a population of policies as the determinant of a kernel matrix over learned behavioral embeddings — i.e. the volume the population spans in behavior space — rather than aggregating pairwise distances. It then adapts the diversity-vs-reward trade-off online, yielding both evolutionary and gradient-based variants that improve exploration without sacrificing return when exploration isn't the bottleneck.

## Key points
- Determinantal (volume-based) diversity replaces pairwise-distance objectives prone to cycling/redundancy.
- Behavioral embeddings are learned, not hand-engineered.
- Online adaptation of the diversity coefficient avoids hurting reward when exploration is unnecessary.
- Both ES and policy-gradient instantiations.

## See also
- [[reward-switching-policy-optimization]]
- [[diverse-psro-behavioural-diversity]]
