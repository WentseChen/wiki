---
title: "Uncertainty-Penalized Reinforcement Learning from Human Feedback with Diverse Reward LoRA Ensembles"
url: https://arxiv.org/abs/2401.00243
type: paper
authors: [Yuanzhao Zhai, Han Zhang, Yu Lei, Yue Yu, Kele Xu, Dawei Feng, Bo Ding, Huaimin Wang]
year: 2023
topics: [rl, nlp]
added: 2026-05-14
arxiv_id: "2401.00243"
---

# Uncertainty-Penalized Reinforcement Learning from Human Feedback with Diverse Reward LoRA Ensembles

**Link:** https://arxiv.org/abs/2401.00243

## Summary

This paper addresses reward overoptimization in RLHF by proposing UP-RLHF: an uncertainty-penalized approach that combines diverse LoRA ensembles for reward model uncertainty quantification with uncertainty-penalized policy optimization. Standard KL regularization in RLHF is insufficient against overoptimization; the authors argue that explicit uncertainty estimation is needed.

The diverse LoRA ensemble is constructed by maximizing the nuclear norm of the ensemble's reward outputs to encourage diversity among ensemble members, which provides reliable uncertainty estimates. Experiments on two human preference datasets show that uncertainty regularization in UP-RLHF substantially mitigates reward overoptimization compared to KL-only baselines. The nuclear norm diversity objective is a novel application of rank-maximization ideas to LoRA ensemble design.

## Key points

- KL regularization alone is insufficient to prevent reward overoptimization in RLHF; explicit uncertainty quantification is needed.
- Diverse LoRA ensembles are constructed by maximizing nuclear norm of reward outputs — a rank-maximization objective encouraging ensemble diversity.
- Uncertainty penalty during policy optimization substantially reduces overoptimization on two human preference datasets.
- Novel connection: nuclear norm maximization for LoRA ensemble diversity inverts the rank-collapse concern — here rank is explicitly boosted.
- Provides a parameter-efficient uncertainty quantification approach for RLHF reward models.

## See also
<!-- [[lora-rlhf-efficiency-regularization]] [[pe-rlhf-parameter-efficient]] -->
