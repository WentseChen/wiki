---
title: "Arbitrary Entropy Policy Optimization Breaks The Exploration Bottleneck of Reinforcement Learning"
url: https://arxiv.org/abs/2510.08141
type: paper
authors: [Chen Wang, Zhaochun Li, Jionghao Bai, Yuzhi Zhang, Shisheng Cui, Zhou Zhao, Yue Wang]
year: 2025
topics: [rl, nlp, theory]
added: 2026-05-14
arxiv_id: "2510.08141"
---

# Arbitrary Entropy Policy Optimization Breaks The Exploration Bottleneck of Reinforcement Learning

**Link:** https://arxiv.org/abs/2510.08141

## Summary

AEPO directly addresses the entropy collapse problem in GRPO, where policy entropy decreases monotonically and exploration disappears. The authors argue existing entropy-regularized methods (entropy-bonus PG, MaxEnt RL) create an unavoidable trade-off between reward and entropy that introduces optimization bias. AEPO reformulates entropy regulation as a policy-gradient problem itself: a REINFORCE regularization term defined over temperature-adjusted samples implicitly modulates entropy without explicitly penalizing the reward objective.

This paper is one of the cleanest formulations of the *policy-side* of the LLM RL collapse problem. It is the dual of the weight-side rank-collapse literature: entropy collapse at the output distribution and rank collapse in the parameter update covariance are two manifestations of the same underlying pathology (low-effective-rank Fisher information / advantage gradient).

## Key points

- Names entropy collapse in GRPO as the *exploration bottleneck* of LLM RL fine-tuning.
- Existing entropy-bonus methods create a reward-vs-entropy trade-off with optimization bias.
- AEPO uses a REINFORCE regularization over temperature-adjusted samples — entropy is regulated implicitly via PG rather than added as a penalty.
- Mechanistic claim: entropy, exploration, and performance are linked rather than antagonistic; precise entropy modulation improves all three.
- Directly relevant to LoRA+RL: entropy collapse at the policy level shrinks the support of the policy gradient, concentrating updates in a low-rank subspace — the upstream cause of LoRA-rank collapse under RL.

## See also
<!-- [[dapo-open-source-rl-system]] [[lora-rank-grpo]] [[rank1-fisher-natural-policy-gradient]] -->
