---
title: "Gradient-Based LoRA Rank Allocation Under GRPO: An Empirical Study"
url: https://arxiv.org/abs/2605.07366
type: paper
authors: [Yash Ganpat Sawant]
year: 2026
topics: [rl, ml]
added: 2026-05-14
arxiv_id: "2605.07366"
---

# Gradient-Based LoRA Rank Allocation Under GRPO: An Empirical Study

**Link:** https://arxiv.org/abs/2605.07366

## Summary

This paper investigates whether adaptive rank allocation strategies for LoRA — which improve efficiency under supervised fine-tuning — transfer to reinforcement learning settings. Testing on Qwen 2.5 1.5B with GSM8K under GRPO, the author finds they do not: proportional rank allocation degrades accuracy by 4.5 points versus uniform allocation (70.0% vs. 74.5%) despite identical parameter budgets. The core finding is that GRPO produces a fundamentally flatter gradient landscape (max-to-min layer importance ratio 2.17x, versus >10x in SFT), meaning gradient-importance signals that drive adaptive allocation under SFT are unreliable under RL.

Two failure mechanisms are identified: (1) all layers carry meaningful gradient signal under GRPO, so no layer is truly idle; (2) a gradient amplification feedback loop where assigning fewer ranks to low-importance layers further suppresses their gradient, widening the importance spread from 2.17x to 3.00x. The results suggest that uniform LoRA rank remains the safer default for RL fine-tuning, and that RL-specific rank allocation strategies require fundamentally different signals than gradient magnitude.

## Key points

- Proportional rank allocation under GRPO loses 4.5% accuracy vs. uniform allocation on GSM8K.
- GRPO gradient landscape is far flatter than SFT: top 30% of layers carry only 35.7% of signal (vs. >80% in SFT).
- Gradient amplification: non-uniform allocation widens layer importance spread from 2.17x to 3.00x, creating a feedback collapse.
- All layers remain functionally important under RL (output formatting, numerical precision, coherence) even when their gradients are small.
- First paper to empirically study adaptive rank allocation specifically under an RL alignment objective (GRPO).

## See also
<!-- [[lora-learns-less-forgets-less]] [[lora-vs-full-finetuning-illusion]] -->
