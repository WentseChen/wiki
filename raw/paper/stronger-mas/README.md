---
title: Stronger-MAS: Multi-Agent Reinforcement Learning for Collaborative LLMs
url: https://arxiv.org/abs/2510.11062
type: paper
authors: [Yujie Zhao, Lanxiang Hu, Yang Wang, Minmin Hou, Hao Zhang]
venue: arXiv
year: 2025
topics: [agents, rl]
added: 2026-05-13
arxiv_id: 2510.11062
---

# Stronger-MAS: Multi-Agent Reinforcement Learning for Collaborative LLMs

**Link:** https://arxiv.org/abs/2510.11062

## Summary
Identifies that vanilla GRPO breaks in MAS where prompts vary by role and turn. Proposes AT-GRPO with agent- and turn-wise grouping plus infra supporting both single-policy and multi-policy training. Reports +50pp planning accuracy and consistent gains on math/coding.

## Key points
- Diagnoses GRPO assumption failures in multi-agent rollouts
- AT-GRPO: agent- and turn-wise grouped advantages
- Single- and multi-policy training infra (PettingLLMs)
- +3.87–7.62% on coding, +9–17.93% on math
- Planning accuracy lifted 14% → 96–99.5%

## See also
<!-- add [[related-slug]] links as connections form -->
