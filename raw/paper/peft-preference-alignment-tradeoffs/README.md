---
title: "A Deep Dive into the Trade-Offs of Parameter-Efficient Preference Alignment Techniques"
url: https://arxiv.org/abs/2406.04879
type: paper
authors: [Megh Thakkar, Quentin Fournier, Matthew D Riemer, Pin-Yu Chen, Amal Zouaq, Payel Das, Sarath Chandar]
venue: ACL 2024
year: 2024
topics: [rl, nlp]
added: 2026-05-14
arxiv_id: "2406.04879"
---

# A Deep Dive into the Trade-Offs of Parameter-Efficient Preference Alignment Techniques

**Link:** https://arxiv.org/abs/2406.04879

## Summary

A systematic empirical study covering 300+ experiments examining how parameter-efficient fine-tuning methods (LoRA, QLoRA) interact with preference alignment techniques (SFT, DPO) across multiple model families (LLaMA-1, Vicuna-v1.3, Mistral-7b, Mistral-7b-Instruct) and two datasets (HH-RLHF, BeaverTails). The study identifies consistent patterns across configurations, providing practitioners with guidelines for LoRA-based preference alignment.

Key findings include cases where SFT outperforms DPO for preference alignment, and evidence that aligning to a distinct preference set can boost performance on downstream tasks. The breadth of the study — four model families, two datasets, two alignment techniques, multiple PEFT configurations — makes it the most comprehensive analysis of LoRA/QLoRA trade-offs in preference alignment to date.

## Key points

- 300+ experiments covering LoRA/QLoRA × SFT/DPO × 4 model families × 2 alignment datasets.
- Cases exist where supervised fine-tuning outperforms DPO for preference alignment.
- Aligning to a distinct preference boosts downstream task performance in certain configurations.
- Published at ACL 2024 (Main); provides practitioner guidelines for PEFT alignment choices.
- Highlights non-trivial interactions between PEFT method, alignment objective, and model architecture.

## See also
<!-- [[lora-rlhf-efficiency-regularization]] [[pe-rlhf-parameter-efficient]] [[lora-learns-less-forgets-less]] -->
