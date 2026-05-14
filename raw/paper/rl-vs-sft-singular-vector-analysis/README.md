---
title: "RL Is Neither a Panacea Nor a Mirage: Understanding Supervised vs. Reinforcement Learning Fine-Tuning for LLMs"
url: https://arxiv.org/abs/2508.16546
type: paper
authors: [Hangzhan Jin, Sicheng Lv, Sifan Wu, Mohammad Hamdaqa]
year: 2025
topics: [rl, nlp]
added: 2026-05-14
arxiv_id: "2508.16546"
---

# RL Is Neither a Panacea Nor a Mirage: Understanding Supervised vs. Reinforcement Learning Fine-Tuning for LLMs

**Link:** https://arxiv.org/abs/2508.16546

## Summary

This paper investigates how SFT and RL fine-tuning (PPO) reshape weight representations through a card game benchmark with controllable distribution shift. The core finding is that RL fine-tuning primarily counteracts SFT-induced directional drift in singular vectors rather than finding genuinely new solutions. Directional shifts of singular vectors matter far more than magnitude changes: the signal concentrates at extreme singular values, and restoring directions for just the top 20% of singular values or first 25% of layers recovers 70–80% of out-of-distribution (OOD) performance.

The study introduces low-rank diagnostic tools (UV merging, shallow-layer resets) to isolate which components drive OOD recovery. A key negative finding: RL recovery fails under severe overfitting or large distribution shift, suggesting RL fine-tuning corrects SFT's directional errors rather than expanding the model's representational capacity.

## Key points

- RL fine-tuning mainly corrects SFT-induced singular-vector drift, not new capacity acquisition.
- Directional changes (singular vector rotation) dominate over magnitude changes (singular value scaling) in driving OOD performance.
- Restoring top-20% singular value directions or first-25% of layers recovers 70–80% of OOD performance.
- RL recovery fails under severe SFT overfitting or large distribution shift.
- Low-rank UV merging and shallow-layer resets are effective diagnostic probes for isolating RL's effect.

## See also
<!-- [[lora-vs-full-finetuning-illusion]] [[lora-rank-grpo]] -->
