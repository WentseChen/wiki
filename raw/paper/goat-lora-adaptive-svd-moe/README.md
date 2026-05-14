---
title: "Make LoRA Great Again: Boosting LoRA with Adaptive Singular Values and Mixture-of-Experts Optimization Alignment"
url: https://arxiv.org/abs/2502.16894
type: paper
authors: [Chenghao Fan, Zhenyi Lu, Sichen Liu, Chengfeng Gu, Xiaoye Qu, Wei Wei, Yu Cheng]
venue: ICML 2025
year: 2025
topics: [ml, nlp]
added: 2026-05-14
arxiv_id: "2502.16894"
---

# Make LoRA Great Again: Boosting LoRA with Adaptive Singular Values and Mixture-of-Experts Optimization Alignment

**Link:** https://arxiv.org/abs/2502.16894

## Summary

GOAT (Great LoRA Mixture-of-Expert) addresses two core failure modes of LoRA: static SVD initialization that fails to adaptively leverage pretrained knowledge, and weight misalignment when combining LoRA with Mixture-of-Experts architectures. The framework introduces SVD-structured MoE that adaptively integrates relevant singular value priors from the pretrained model, plus theoretical scaling factors to align LoRA-MoE optimization dynamics with fully fine-tuned MoE systems.

Evaluated across 25 datasets spanning language understanding, reasoning, image classification, and generation, GOAT closes the gap with full fine-tuning while maintaining parameter efficiency. The paper's core insight is that static low-rank subspace selection (standard LoRA) is suboptimal because the relevant singular components vary across inputs and tasks — adaptive selection via MoE routing recovers this lost capacity.

## Key points

- Identifies two LoRA failure modes: static SVD initialization and optimization misalignment in LoRA-MoE systems.
- SVD-structured MoE adaptively routes to relevant singular value priors from the pretrained weight spectrum.
- Derives theoretical scaling factors aligning LoRA-MoE gradient dynamics with full fine-tuning.
- Tested on 25 datasets across multiple modalities; closes the LoRA-vs-full-FT gap.
- Accepted at ICML 2025; provides both theory and strong empirical validation.

## See also
<!-- [[lora-learns-less-forgets-less]] [[essa-evolutionary-strategies-alignment]] [[lora-vs-full-finetuning-illusion]] -->
