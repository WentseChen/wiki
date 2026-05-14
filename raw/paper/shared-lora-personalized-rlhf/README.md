---
title: "A Shared Low-Rank Adaptation Approach to Personalized RLHF"
url: https://arxiv.org/abs/2503.19201
type: paper
authors: [Renpu Liu, Peng Wang, Donghao Li, Cong Shen, Jing Yang]
venue: AISTATS 2025
year: 2025
topics: [rl, nlp]
added: 2026-05-14
arxiv_id: "2503.19201"
---

# A Shared Low-Rank Adaptation Approach to Personalized RLHF

**Link:** https://arxiv.org/abs/2503.19201

## Summary

This paper extends RLHF to handle heterogeneous human preferences by applying LoRA in the aggregated parameter space of all personalized reward functions. Rather than assuming a single homogeneous preference, the framework allows each user to have individual reward functions while exploiting shared low-rank structure across users to enable learning from limited local datasets.

The approach provides sample complexity guarantees for personalized RLHF — a theoretical contribution distinguishing it from purely empirical work. By applying LoRA in the shared aggregated parameter space, the method efficiently captures both common alignment signals and user-specific deviations, demonstrating effectiveness on real-world preference datasets.

## Key points

- Personalizes RLHF by applying LoRA in the aggregated parameter space of all personalized reward functions.
- Exploits shared low-rank structure across users to enable learning from limited local preference data.
- Provides sample complexity guarantees for personalized RLHF — a theoretical contribution.
- Demonstrated on real-world preference datasets; balances personalization with data efficiency.
- Published at AISTATS 2025; connects LoRA to the theoretical study of heterogeneous preference alignment.

## See also
<!-- [[pe-rlhf-parameter-efficient]] [[peft-preference-alignment-tradeoffs]] -->
