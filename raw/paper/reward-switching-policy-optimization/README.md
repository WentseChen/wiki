---
title: Continuously Discovering Novel Strategies via Reward-Switching Policy Optimization
url: https://arxiv.org/abs/2204.02246
type: paper
authors: [Zihan Zhou, Wei Fu, Bingliang Zhang, Yi Wu]
venue: ICLR
year: 2022
topics: [rl, agents]
added: 2026-05-12
arxiv_id: 2204.02246
---

# Continuously Discovering Novel Strategies via Reward-Switching Policy Optimization

**Link:** https://arxiv.org/abs/2204.02246

## Summary

RSPO is an iterative RL paradigm that discovers diverse behavioral strategies by sequentially finding novel locally-optimal policies distinct from existing ones. It dynamically switches between extrinsic task reward and an intrinsic diversity reward depending on whether a sampled trajectory looks novel or resembles previously found policies, steering exploration toward undiscovered solutions.

Empirical results span particle environments, MuJoCo continuous control, multi-agent games, and StarCraft II — showing the method can recover qualitatively different strategies a single RL run typically collapses onto one of.

## Key points
- Dual-reward mechanism: extrinsic reward on novel trajectories, intrinsic diversity reward on trajectories that resemble existing policies.
- Trajectory-level (not state-level) novelty measurement determines which reward signal is active.
- Iterative: builds a population of locally-optimal policies one at a time rather than converging to a single solution.
- Validated across single-agent, multi-agent cooperative, and competitive (StarCraft II) settings.

## See also
- [[diverse-psro-behavioural-diversity]] — diversity in PSRO populations
- [[neupl-neural-population-learning]] — population learning with shared net
