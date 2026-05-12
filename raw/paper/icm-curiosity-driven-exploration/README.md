---
title: Curiosity-driven Exploration by Self-supervised Prediction
url: https://arxiv.org/abs/1705.05363
type: paper
authors: [Deepak Pathak, Pulkit Agrawal, Alexei A. Efros, Trevor Darrell]
venue: ICML
year: 2017
topics: [rl]
added: 2026-05-12
arxiv_id: 1705.05363
---

# Curiosity-driven Exploration by Self-supervised Prediction (ICM)

**Link:** https://arxiv.org/abs/1705.05363

## Summary

ICM defines intrinsic curiosity as the error of a forward dynamics model operating in a feature space learned by an inverse dynamics model. The inverse-model feature space filters out environment changes the agent cannot affect, so curiosity rewards focus on agent-relevant novelty — enabling exploration in sparse-reward and pure-exploration regimes on VizDoom and Super Mario.

## Key points
- Curiosity = forward-model prediction error in a learned feature space.
- Inverse dynamics model learns agent-controllable features; ignores distractors.
- Strong results on sparse-reward and reward-free exploration tasks.
- Canonical intrinsic-motivation baseline; precursor to RND, NGU, and trajectory-novelty signals in RSPO.

## See also
- [[reward-switching-policy-optimization]]
