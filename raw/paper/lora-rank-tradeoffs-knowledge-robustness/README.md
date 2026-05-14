---
title: "How Much is Too Much? Exploring LoRA Rank Trade-offs for Retaining Knowledge and Domain Robustness"
url: https://arxiv.org/abs/2512.15634
type: paper
authors: [Darshita Rathore, Vineet Kumar, Chetna Bansal, Anindya Moitra]
venue: AACL-IJCNLP 2025
year: 2025
topics: [ml, nlp]
added: 2026-05-14
arxiv_id: "2512.15634"
---

# How Much is Too Much? Exploring LoRA Rank Trade-offs for Retaining Knowledge and Domain Robustness

**Link:** https://arxiv.org/abs/2512.15634

## Summary

This paper performs a comprehensive rank sweep to quantify the trade-off between SFT and PEFT (LoRA) across multiple reasoning and recall datasets. The study examines how LLMs adapt to downstream tasks under varying LoRA rank configurations, measuring both in-domain performance and out-of-domain generalization. Internal representation changes are analyzed through spectral features and attention pattern modifications to understand structural shifts in the model.

Key findings show that LoRA can match or exceed standard fine-tuning on certain reasoning tasks at optimal rank configurations, but that higher ranks do not monotonically improve performance — there is a "too much" threshold beyond which forgetting accelerates without proportional gains. Spectral analysis of weight matrices reveals structural shifts correlated with domain robustness changes.

## Key points

- LoRA can match or exceed full SFT on some reasoning tasks at optimal rank, but performance stagnates or declines at higher ranks.
- Rank sweep reveals a non-monotonic relationship: increasing rank past an optimum accelerates forgetting without proportional in-domain gains.
- Spectral features and attention pattern analysis reveal structural shifts in representations correlated with OOD robustness.
- Trade-off between domain adaptation and knowledge retention is rank-dependent and task-specific.
- Published at AACL-IJCNLP 2025; provides practical guidance on rank selection for practitioners.

## See also
<!-- [[lora-learns-less-forgets-less]] [[lora-vs-full-finetuning-illusion]] -->
