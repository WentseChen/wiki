---
title: "Measuring the Intrinsic Dimension of Objective Landscapes"
url: https://arxiv.org/abs/1804.08838
type: paper
authors: [Chunyuan Li, Heerad Farkhoor, Rosanne Liu, Jason Yosinski]
venue: ICLR 2018
year: 2018
topics: [theory, rl]
added: 2026-05-14
arxiv_id: 1804.08838
---

# Measuring the Intrinsic Dimension of Objective Landscapes

**Link:** https://arxiv.org/abs/1804.08838

## Summary

This ICLR 2018 seminal paper introduces the concept of *intrinsic dimension* of an objective landscape: the minimum dimensionality of a randomly-oriented subspace in which optimization first finds a solution. Networks are trained not in their native parameter space but in progressively larger random subspaces, and the smallest dimension at which a solution emerges is defined as the intrinsic dimension. The method reveals that many problems have far smaller intrinsic dimensions than their parameter counts suggest, and that once the parameter space is large enough, extra parameters mainly expand the solution manifold rather than solving harder problems.

The paper shows that architecturally different models solving the same dataset share similar intrinsic dimensions, and enables cross-domain difficulty comparisons: solving the inverted pendulum is ~100× easier than MNIST classification, and playing Pong is comparable to CIFAR-10. It also provides >100× network compression in some cases by parameterizing solutions in a low-dimensional subspace.

## Key points

- Intrinsic dimension = min dimensionality of a random subspace where gradient descent finds a solution.
- Architecturally diverse models share similar intrinsic dimensions on the same task, decoupling architecture from problem difficulty.
- Cross-domain comparisons: RL tasks (inverted pendulum) are ~100× easier than MNIST; Atari Pong ≈ CIFAR-10 difficulty.
- Extra parameters beyond the intrinsic threshold expand the solution manifold but do not reduce intrinsic dimension.
- Foundational for LoRA and PEFT: motivates constraining fine-tuning to a low-dimensional subspace of parameter space.

## See also
- [[intrinsic-dim-lm-finetuning]] — direct follow-up applying intrinsic dimension to LM fine-tuning
