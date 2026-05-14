---
title: "Intrinsic Dimensionality Explains the Effectiveness of Language Model Fine-Tuning"
url: https://arxiv.org/abs/2012.13255
type: paper
authors: [Armen Aghajanyan, Luke Zettlemoyer, Sonal Gupta]
venue: ACL 2021
year: 2021
topics: [nlp, theory]
added: 2026-05-14
arxiv_id: 2012.13255
---

# Intrinsic Dimensionality Explains the Effectiveness of Language Model Fine-Tuning

**Link:** https://arxiv.org/abs/2012.13255

## Summary

This foundational paper establishes that pretrained language models have remarkably low intrinsic dimensionality — the minimal number of free parameters needed to achieve near-full-model fine-tuning performance. By optimizing only ~200 parameters randomly projected back into the full weight space, a RoBERTa model reaches 90% of full fine-tuning performance on MRPC. Pre-training is shown to implicitly minimize intrinsic dimension, and larger models exhibit lower intrinsic dimension after equivalent training, directly motivating the LoRA design philosophy.

The authors connect intrinsic dimensionality to compression-based generalization bounds that scale with task complexity rather than total parameter count, explaining why vanilla gradient descent avoids overfitting despite extreme parameter-to-data ratios. This provides the theoretical grounding for why rank-constrained fine-tuning (e.g., LoRA) works: the objective landscape is effectively low-dimensional even when the parameter space is enormous.

## Key points

- Pretrained LMs can be fine-tuned to ~90% of full performance by optimizing only ~200 parameters in a random subspace projection.
- Pre-training implicitly reduces intrinsic dimension; larger models have lower intrinsic dimension after equivalent pre-training steps.
- Compression-based generalization bounds tied to intrinsic dimension (not full parameter count) explain fine-tuning efficiency.
- Intrinsic dimension varies by task difficulty, providing a quantitative measure of task complexity.
- Foundational motivation for LoRA and subsequent PEFT methods: fine-tuning solutions lie in a low-dimensional subspace of parameter space.

## See also
- [[lora-ntk-no-spurious-minima]]
- [[lora-convergence-implicit-bias]]
