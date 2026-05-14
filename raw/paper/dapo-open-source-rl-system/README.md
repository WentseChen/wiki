---
title: "DAPO: An Open-Source LLM Reinforcement Learning System at Scale"
url: https://arxiv.org/abs/2503.14476
type: paper
authors: [Qiying Yu, Zheng Zhang, Ruofei Zhu, Yufeng Yuan, Xiaochen Zuo, et al.]
year: 2025
topics: [rl, nlp, systems]
added: 2026-05-14
arxiv_id: "2503.14476"
---

# DAPO: An Open-Source LLM Reinforcement Learning System at Scale

**Link:** https://arxiv.org/abs/2503.14476

## Summary

DAPO (Decoupled Clip and Dynamic sAmpling Policy Optimization) is an open-source large-scale RL system for reasoning LLMs that explicitly names and addresses the *entropy collapse* failure mode of vanilla PPO/GRPO. When applied naively to long-CoT RL with Qwen2.5-32B, GRPO's policy entropy decreases rapidly and sampled responses become nearly identical within a group — eliminating the diversity that group-relative advantage requires. DAPO combines four key techniques (decoupled clip-higher, dynamic sampling, token-level policy gradient loss, and overlong reward shaping) to mitigate this collapse and achieves 50 points on AIME 2024.

DAPO is the canonical reference for entropy collapse in RLHF/RLVR — it is the bridge between the rank-collapse literature on weight matrices and the well-documented diversity collapse observed at the policy/output level during GRPO training. The decoupled clip in particular raises the clip upper bound for low-probability tokens, preserving exploration directions that vanilla PPO ratio clipping would suppress.

## Key points

- Names entropy collapse as a primary failure mode of GRPO: policy entropy drops monotonically, group-sampled responses converge to near-identical outputs, exploration vanishes.
- Decoupled "Clip-Higher": raises the upper clip ratio for low-probability tokens to allow exploration without sacrificing stability.
- Dynamic sampling: filters prompts whose group rollouts all share the same reward (all-correct / all-wrong), preserving gradient signal.
- Token-level policy gradient loss + overlong reward shaping mitigate length-bias artifacts of long-CoT RL.
- Achieves 50 points on AIME 2024 with Qwen2.5-32B base; fully open-source training code on the verl framework.

## See also
<!-- [[lora-rank-grpo]] [[lora-rlhf-efficiency-regularization]] -->
