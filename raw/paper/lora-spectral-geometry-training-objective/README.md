---
title: "Spectral Geometry of LoRA Adapters Encodes Training Objective and Predicts Harmful Compliance"
url: https://arxiv.org/abs/2604.08844
type: paper
authors: [Roi Paul]
year: 2026
topics: [ml, nlp]
added: 2026-05-14
arxiv_id: "2604.08844"
---

# Spectral Geometry of LoRA Adapters Encodes Training Objective and Predicts Harmful Compliance

**Link:** https://arxiv.org/abs/2604.08844

## Summary

This paper shows that the spectral geometry of LoRA weight deltas — per-layer statistics including stable rank, singular-value entropy, effective rank, and singular-vector alignment — encodes which fine-tuning objective was applied, and predicts downstream harmful behavior. Testing on Llama-3.2-3B-Instruct with 38 adapters across SFT, DPO, and steering variants, logistic regression on spectral features achieves AUC ~1.00 for within-method training objective classification and ordinal severity ranking (Spearman ρ ≥ 0.956).

Key structural findings: query-projection weights signal whether drift occurred; value-projection weights identify the specific objective. However, cross-method generalization fails entirely — a detector trained on DPO adapters assigns lower drift scores to steering adapters than to DPO, underscoring the need for method-specific calibration. The behavioral arm confirms spectral severity correlates with harmful compliance (ASR 0.266 vs. baseline 0.112) with near-perfect dose-response (ρ = 0.986).

## Key points

- Spectral features (effective rank, stable rank, singular-value entropy) of LoRA deltas reliably identify training objectives within a method family (AUC ~1.00).
- Query-weight projections encode drift occurrence; value-weight projections encode objective identity.
- Harmful compliance correlates with spectral severity with near-perfect dose-response (ρ = 0.986).
- Cross-method generalization fails: DPO-trained detectors cannot recognize steering-based adapters.
- First paper to use LoRA spectral geometry as an adapter safety/alignment monitoring signal.

## See also
<!-- [[lora-vs-full-finetuning-illusion]] [[lora-rank-grpo]] -->
