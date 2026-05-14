---
title: "Exploring the impact of low-rank adaptation on the performance, efficiency, and regularization of RLHF"
url: https://arxiv.org/abs/2309.09055
type: paper
authors: [Simeng Sun, Dhawal Gupta, Mohit Iyyer]
year: 2023
topics: [rl, nlp]
added: 2026-05-14
arxiv_id: "2309.09055"
---

# Exploring the impact of low-rank adaptation on the performance, efficiency, and regularization of RLHF

**Link:** https://arxiv.org/abs/2309.09055

## Summary

An early foundational study demonstrating efficient RLHF via LoRA (PPO), aligning LLaMA 7B on the Alpaca dataset using only two A100 GPUs by tuning just 0.2% of parameters. Despite this extreme parameter efficiency, the LoRA-PPO approach outperforms the publicly released AlpacaFarm checkpoint, establishing that LoRA is a viable drop-in for RLHF policy training.

Key regularization findings: removing the KL penalty term does not diminish performance under the LoRA setup (suggesting LoRA's low-rank constraint already acts as an implicit regularizer); Jensen-Shannon divergence yields improvements over KL; and LoRA-based PPO largely mitigates the factuality degradation typically caused by PPO training. The paper releases code and pretrained checkpoints.

## Key points

- LoRA-PPO aligns LLaMA 7B on 2× A100s using only 0.2% of parameters, outperforming full AlpacaFarm checkpoint.
- Removing the KL penalty does not hurt performance under LoRA — suggests implicit regularization from the low-rank constraint.
- Jensen-Shannon divergence outperforms standard KL divergence in the LoRA-RLHF setting.
- LoRA largely mitigates factuality degradation caused by PPO training — an important safety benefit.
- Foundational paper for the LoRA+RLHF workflow; widely cited as the first efficient LoRA-PPO implementation.

## See also
<!-- [[lora-rank-grpo]] [[pe-rlhf-parameter-efficient]] -->
