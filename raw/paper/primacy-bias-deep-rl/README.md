---
title: The Primacy Bias in Deep Reinforcement Learning
url: https://arxiv.org/abs/2205.07802
type: paper
authors: [Evgenii Nikishin, Max Schwarzer, Pierluca D'Oro, Pierre-Luc Bacon, Aaron Courville]
venue: ICML 2022
year: 2022
topics: [rl, continuous-learning]
added: 2026-05-12
arxiv_id: 2205.07802
---

# The Primacy Bias in Deep Reinforcement Learning

**Link:** https://arxiv.org/abs/2205.07802

## Summary
Nikishin et al. identify a "primacy bias": deep RL agents trained with high update-to-data ratios irreversibly overfit to their earliest few thousand transitions, after which more gradient steps actively hurt. The fix is brutally simple — every N environment steps, reset the last few layers (or the whole network) of the agent while keeping the replay buffer. This single trick lifts SAC, DrQ, and SPR by large margins and reframes "more updates per env step" as a viable scaling axis.

For the Dohare paper, this is the closest RL-side cousin: same phenomenon (loss of trainability under non-stationarity), same family of solution (reinit a chunk of the net), but coarser (whole-layer episodic resets vs. per-unit continual reinitialization).

## Key points
- Frames a previously diffuse RL pathology as a single "primacy bias" phenomenon.
- Periodic full-layer resets recover plasticity without irreparable damage; post-reset dip recovers within thousands of steps.
- Higher replay ratios become beneficial only after enabling resets.
- Works in both discrete (Atari-100k) and continuous (DMC) regimes.

## See also
<!-- [[plasticity]] · [[dormant-neuron-phenomenon]] · [[plasticity-injection-drl]] -->
