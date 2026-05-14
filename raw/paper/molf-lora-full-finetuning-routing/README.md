---
title: "Beyond LoRA vs. Full Fine-Tuning: Gradient-Guided Optimizer Routing for LLM Adaptation"
url: https://arxiv.org/abs/2605.07111
type: paper
authors: [Haozhan Tang, Xiuqi Zhu, Xinyin Zhang, Boxun Li, Virginia Smith, Kevin Kuo]
year: 2026
topics: [ml, nlp]
added: 2026-05-14
arxiv_id: "2605.07111"
---

# Beyond LoRA vs. Full Fine-Tuning: Gradient-Guided Optimizer Routing for LLM Adaptation

**Link:** https://arxiv.org/abs/2605.07111

## Summary

MoLF (Mixture of LoRA and Full Fine-Tuning) proposes a unified framework that dynamically routes gradient updates between LoRA and full fine-tuning at the optimizer level, bypassing the need to statically choose one approach. The routing decision is guided by per-layer gradient statistics — layers where LoRA is sufficient receive low-rank updates, while layers requiring higher effective rank receive full fine-tuning updates. This directly addresses the gap documented in papers like "LoRA Learns Less and Forgets Less" without discarding LoRA's parameter efficiency entirely.

For memory-constrained settings, MoLF-Efficient routes among multiple LoRA experts with varying ranks instead of between LoRA and full FT. Results show MoLF is competitive across all tested settings, while MoLF-Efficient outperforms prior adaptive rank allocation approaches — including under GRPO-style RL settings where adaptive rank allocation typically fails.

## Key points

- Routes gradient updates between LoRA and full FT at the optimizer level using per-layer gradient statistics.
- MoLF-Efficient variant routes among LoRA experts of varying ranks for memory-constrained settings.
- Addresses the "LoRA underperforms" gap without fully discarding parameter efficiency.
- Outperforms prior adaptive rank methods, including in RL fine-tuning contexts.
- Complementary to lora-rank-grpo findings: when gradient signals fail for rank allocation, full FT routing is the escape valve.

## See also
<!-- [[lora-learns-less-forgets-less]] [[lora-rank-grpo]] [[lora-vs-full-finetuning-illusion]] -->
