---
title: A Unified Game-Theoretic Approach to Multiagent Reinforcement Learning
url: https://arxiv.org/abs/1711.00832
type: paper
authors: [Marc Lanctot, Vinicius Zambaldi, Audrunas Gruslys, Angeliki Lazaridou, Karl Tuyls, Julien Perolat, David Silver, Thore Graepel]
venue: NeurIPS
year: 2017
topics: [rl, game-theory, agents]
added: 2026-05-11
arxiv_id: 1711.00832
---

# A Unified Game-Theoretic Approach to Multiagent Reinforcement Learning

**Link:** https://arxiv.org/abs/1711.00832

## Summary
Argues independent RL agents overfit to their training opponents and proposes a unified algorithm — Policy Space Response Oracles (PSRO) — that combines deep RL (for approximate best responses) with empirical game-theoretic analysis (for meta-strategies over a growing population of policies). Generalizes fictitious play and double oracle, and introduces "joint-policy correlation" to quantify the overfitting effect in multiagent settings.

## Key points
- Independent RL (InRL) policies overfit to co-trained opponents and fail to generalize.
- Introduces joint-policy correlation (JPC) as a diagnostic for multiagent overfitting.
- PSRO = iterative best-response training against a meta-distribution over prior policies.
- Unifies fictitious play, double oracle, and self-play under one framework.
- Decoupled meta-solvers reduce memory and scale to gridworld coordination + Leduc poker.

## See also
<!-- [[<related-slug>]] — optional, link if obvious relatives exist -->
