---
title: Loss of plasticity in deep continual learning
url: https://www.nature.com/articles/s41586-024-07711-7
type: paper
authors: [Shibhansh Dohare, J. Fernando Hernandez-Garcia, Qingfeng Lan, Parash Rahman, A. Rupam Mahmood, Richard S. Sutton]
venue: Nature
year: 2024
topics: [continuous-learning, rl, ml]
added: 2026-05-12
---

# Loss of plasticity in deep continual learning

**Link:** https://www.nature.com/articles/s41586-024-07711-7

## Summary
Standard deep-learning methods gradually lose plasticity in continual-learning settings — eventually learning no better than a shallow network — across both supervised (Continual ImageNet, permuted MNIST) and reinforcement-learning benchmarks, robust across architectures and optimizers. The paper proposes **continual backpropagation**, a tiny modification of SGD that continually reinitializes a small fraction of the least-used hidden units, restoring and maintaining plasticity indefinitely. Result: a fundamental, previously underappreciated failure mode of deep nets in non-stationary settings, with a near drop-in fix.

## Key points
- Plasticity loss is pervasive: shown on Continual ImageNet, permuted MNIST, and continual RL — independent of optimizer (SGD, Adam) and architecture (MLPs, CNNs, ResNets).
- Symptoms: growing fraction of "dead"/dormant units, exploding weight magnitudes, vanishing effective rank of representations.
- Standard regularizers (L2, dropout) help partially; the cleanest fix is generate-and-test style unit reinitialization.
- Continual backpropagation = backprop + a "utility" score per hidden unit; the lowest-utility fraction is randomly reinitialized each step.
- The method preserves plasticity over millions of tasks/updates while matching or beating baselines on accuracy.

## See also
<!-- related slugs: none yet in wiki -->
