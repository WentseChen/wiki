---
title: "LoRA Learns Less and Forgets Less"
url: https://arxiv.org/abs/2405.09673
type: paper
authors: [Dan Biderman, Jacob Portes, Jose Javier Gonzalez Ortiz, Mansheej Paul, Philip Greengard, Connor Jennings, Daniel King, Sam Havens, Vitaliy Chiley, Jonathan Frankle, Cody Blakeney, John P. Cunningham]
venue: Transactions on Machine Learning Research (TMLR)
year: 2024
topics: [ml, nlp]
added: 2026-05-14
arxiv_id: "2405.09673"
---

# LoRA Learns Less and Forgets Less

**Link:** https://arxiv.org/abs/2405.09673

## Summary

This TMLR paper provides a systematic empirical comparison of LoRA vs. full fine-tuning across two target domains (programming and mathematics), two data regimes (instruction fine-tuning ~100K pairs, continued pretraining on 20B tokens). The headline result: in standard low-rank settings, LoRA substantially underperforms full fine-tuning on in-domain tasks. However, LoRA better maintains base model performance on out-of-domain tasks — it "learns less and forgets less."

A key mechanistic finding: full fine-tuning learns weight perturbations whose effective rank is 10–100x greater than typical LoRA configurations, which likely explains the performance gap. LoRA mitigates forgetting more effectively than standard regularization techniques (weight decay, dropout) and maintains more diverse generations. The paper concludes with practical best-practice guidelines for LoRA fine-tuning.

## Key points

- LoRA substantially underperforms full fine-tuning in standard low-rank settings on in-domain tasks (coding, math).
- LoRA better preserves out-of-domain base model performance — learns less, forgets less.
- Full fine-tuning learns weight updates with effective rank 10–100x higher than typical LoRA rank.
- LoRA mitigates forgetting more than weight decay or dropout regularization.
- Published in TMLR 2024 (Featured Certification); widely cited as the canonical LoRA-vs-full-FT comparison.

## See also
<!-- [[lora-vs-full-finetuning-illusion]] [[lora-rank-grpo]] -->
