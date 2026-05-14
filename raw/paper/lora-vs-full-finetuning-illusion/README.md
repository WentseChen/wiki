---
title: "LoRA vs Full Fine-tuning: An Illusion of Equivalence"
url: https://arxiv.org/abs/2410.21228
type: paper
authors: [Reece Shuttleworth, Jacob Andreas, Antonio Torralba, Pratyusha Sharma]
year: 2024
topics: [ml, nlp]
added: 2026-05-14
arxiv_id: "2410.21228"
---

# LoRA vs Full Fine-tuning: An Illusion of Equivalence

**Link:** https://arxiv.org/abs/2410.21228

## Summary

This paper challenges the widely held assumption that LoRA and full fine-tuning produce functionally equivalent weight updates. Via spectral analysis (SVD) of fine-tuned weight matrices, the authors show that LoRA introduces "intruder dimensions" — new high-ranking singular vectors that do not appear in fully fine-tuned models. These intruder dimensions causally drive catastrophic forgetting: the model loses pre-training knowledge precisely in the directions spanned by these anomalous singular vectors. Scaling down intruder dimension magnitudes post-hoc recovers pre-training performance with minimal task loss.

The problem compounds in continual learning: sequential LoRA fine-tuning accumulates intruder dimensions across tasks, causing LoRA to substantially underperform full fine-tuning in multi-task settings. The work provides a spectral diagnostic that quantifies LoRA-induced forgetting and motivates better initialization or merging strategies to suppress intruder dimensions.

## Key points

- LoRA and full fine-tuning produce qualitatively different SVD spectra; LoRA inserts high-rank singular vectors absent in full FT.
- These "intruder dimensions" causally localize forgetting — intervening on them post-hoc restores pre-training knowledge.
- Continual sequential LoRA fine-tuning compounds intruder accumulation, leading to severe multi-task degradation.
- Scaling down intruder singular values post-fine-tuning preserves task performance while recovering pre-training generalization.
- Results question the common claim that LoRA ≈ full fine-tuning at equivalent rank; they converge to geometrically distinct solutions.

## See also
<!-- [[lora-rank-grpo]] [[lora-learns-less-forgets-less]] -->
