---
title: Diversity is All You Need - Learning Skills without a Reward Function
url: https://arxiv.org/abs/1802.06070
type: paper
authors: [Benjamin Eysenbach, Abhishek Gupta, Julian Ibarz, Sergey Levine]
venue: ICLR
year: 2019
topics: [rl]
added: 2026-05-12
arxiv_id: 1802.06070
---

# Diversity is All You Need: Learning Skills without a Reward Function

**Link:** https://arxiv.org/abs/1802.06070

## Summary

DIAYN is an unsupervised RL method that discovers diverse skills without any task reward, by maximizing the mutual information between a latent skill variable and the states the policy visits while keeping the policy maximum-entropy. The resulting skill set (walking, jumping, etc.) emerges purely from the information-theoretic objective and transfers as initialization or as a hierarchical action space for downstream tasks.

## Key points
- Unsupervised — no extrinsic reward used during skill learning.
- Information-theoretic objective: maximize I(skill ; state) while maximizing entropy over actions.
- Pretrained skills transfer to downstream tasks via finetuning or as options.
- Canonical reference for mutual-information-based skill discovery.

## See also
- [[reward-switching-policy-optimization]]
- [[dads-dynamics-aware-skills]]
