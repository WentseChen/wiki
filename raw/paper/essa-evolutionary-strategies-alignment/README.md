---
title: "ESSA: Evolutionary Strategies for Scalable Alignment"
url: https://arxiv.org/abs/2507.04453
type: paper
authors: [Daria Korotyshova, Boris Shaposhnikov, Alexey Malakhov, Alexey Khokhulin, Nikita Surnachev, Kirill Ovcharenko, George Bredis, Alexey Gorbatovski, Viacheslav Sinii, Daniil Gavrilov]
year: 2025
topics: [rl, nlp]
added: 2026-05-14
arxiv_id: "2507.04453"
---

# ESSA: Evolutionary Strategies for Scalable Alignment

**Link:** https://arxiv.org/abs/2507.04453

## Summary

ESSA proposes gradient-free LLM alignment by applying evolutionary search over the singular values of LoRA adapter matrices via SVD decomposition. Rather than using gradient-based RL methods (PPO, GRPO), which require complex distributed training and large memory budgets, ESSA treats only the singular values of each adapter as the optimization target, making the search space small enough for evolutionary algorithms while operating in quantized (INT4/INT8) inference mode.

The method achieves strong empirical results: +12.6% on GSM8K and +14.8% on PRM800K for Qwen2.5-Math-7B, and +22.5% on IFEval for LLaMA3.1-8B versus gradient-based baselines. ESSA is significant for the LoRA/RL intersection because it implicitly demonstrates that the singular values of LoRA adapters encode the bulk of alignment information, supporting the hypothesis that effective alignment requires only a low-dimensional subspace within LoRA weight space.

## Key points

- Optimizes only singular values of LoRA adapter SVD — dramatically reducing the search space for evolutionary alignment.
- Gradient-free: no backpropagation, no reward model, works in INT4/INT8 quantized inference mode.
- Matches GRPO baselines on math and instruction-following benchmarks with reduced engineering overhead.
- Implicitly shows singular values are the primary carrier of alignment information in LoRA adapters.
- Scales better than gradient-based methods on very large models due to reduced memory and complexity.

## See also
<!-- [[lora-spectral-geometry-training-objective]] [[lora-rank-grpo]] [[essa-goat-lora-adaptive-svd]] -->
