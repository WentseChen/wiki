# nlp

Language models, training, alignment, prompting, evaluation.

## Overview

<!-- short overview, maintained by LLM as the topic grows -->

## Key concepts

<!-- bullet list of [[concept-slug]] links into articles/concepts/ -->

## Recent

- [[aepo-arbitrary-entropy-policy-optimization]] — AEPO reformulates entropy regulation as a PG problem via REINFORCE on temperature-adjusted samples; avoids reward-vs-entropy trade-off; dual of weight-side rank collapse. *Wang et al., 2025.*
- [[dapo-open-source-rl-system]] — DAPO names entropy collapse as core GRPO failure; decoupled clip-higher + dynamic sampling restore exploration; 50 pts AIME 2024 on Qwen2.5-32B. *Yu et al., 2025.*
- [[rmt-transformer-singular-values]] — RMT baseline (Marchenko-Pastur) reveals learned structure at both spectrum ends in transformers; small SVs matter; fine-tuning shifts importance toward extremes. *Staats et al., 2024.*
- [[lora-one-singular-subspace]] — Proves LoRA adapters align to singular subspaces of one-step full gradient; LoRA-One init achieves linear convergence; explains rank collapse under sparse-reward RL. *Zhang et al., 2025 (ICML oral).*
- [[intrinsic-dim-lm-finetuning]] — Pretrained LMs have very low intrinsic dimensionality; ~200 params in random subspace achieves 90% of full FT; compression-based generalization bounds. *Aghajanyan et al., 2021 (ACL).*
- [[molf-lora-full-finetuning-routing]] — MoLF routes gradient updates between LoRA and full FT at optimizer level; MoLF-Efficient routes among variable-rank LoRA experts. *Tang et al., 2026.*
- [[remix-rl-routing-mixture-loras]] — Routing collapse in Mixture-of-LoRAs fixed via RL gradient estimation on non-learnable routers; enforces balanced adapter utilization. *Qiu et al., 2026 (ICLR).*
- [[shared-lora-personalized-rlhf]] — LoRA in aggregated reward parameter space handles heterogeneous preferences; sample complexity guarantees for personalized RLHF. *Liu et al., 2025 (AISTATS).*
- [[peft-preference-alignment-tradeoffs]] — 300+ experiments: LoRA/QLoRA × SFT/DPO; SFT sometimes beats DPO; non-trivial PEFT-alignment interactions across model families. *Thakkar et al., 2024 (ACL).*
- [[up-rlhf-diverse-lora-ensembles]] — Diverse LoRA ensembles (nuclear norm diversity) quantify reward uncertainty; uncertainty penalty mitigates RLHF overoptimization. *Zhai et al., 2023.*
- [[pe-rlhf-parameter-efficient]] — LoRA-based PE-RLHF matches full RLHF on 6 tasks; 90% faster reward model training, 50% memory savings. *Sidahmed et al., 2024.*
- [[lora-rlhf-efficiency-regularization]] — LoRA-PPO aligns LLaMA 7B on 2 A100s (0.2% params); KL penalty unneeded (implicit regularization); mitigates PPO factuality degradation. *Sun et al., 2023.*
- [[goat-lora-adaptive-svd-moe]] — GOAT: SVD-structured MoE routes to relevant singular value priors; closes LoRA-vs-full-FT gap on 25 datasets. *Fan et al., 2025 (ICML).*
- [[essa-evolutionary-strategies-alignment]] — Gradient-free alignment via evolutionary search over LoRA singular values; matches GRPO without backprop; shows SVs encode alignment info. *Korotyshova et al., 2025.*
- [[lora-rank-tradeoffs-knowledge-robustness]] — LoRA rank has non-monotonic effect: past an optimum, higher rank accelerates forgetting with no in-domain gain; spectral analysis confirms. *Rathore et al., 2025 (AACL).*
- [[lora-learns-less-forgets-less]] — LoRA underperforms full FT on in-domain tasks; full FT learns 10–100x higher effective rank; LoRA forgets less but learns less. *Biderman et al., 2024 (TMLR).*
- [[rl-vs-sft-singular-vector-analysis]] — RL fine-tuning corrects SFT-induced singular-vector drift; direction changes dominate magnitude; top-20% SVD directions recover 70-80% OOD perf. *Jin et al., 2025.*
- [[lora-spectral-geometry-training-objective]] — Spectral features (effective rank, stable rank) of LoRA deltas classify training objective at AUC~1.00 and predict harmful compliance. *Paul, 2026.*
- [[lora-vs-full-finetuning-illusion]] — LoRA inserts "intruder dimensions" (anomalous high-rank singular vectors) that causally drive forgetting; LoRA ≠ full FT spectrally. *Shuttleworth et al., 2024.*
- [[multi-agents-debate]] — Adversarial debate + judge mitigates Degeneration of Thoughts in single-agent self-reflection. *Liang et al., 2023.*
- [[openrlhf]] — Ray + vLLM RLHF; PPO / REINFORCE++ / GRPO / RLOO; sync/async/hybrid; MARTI's parent codebase. *OpenRLHF, 2024.*
- [[verl-hybridflow]] — Hybrid-controller RL post-training; FSDP/Megatron/vLLM integration; backbone for many agentic-RL frameworks. *ByteDance Seed et al., 2024.*
<!-- newest at top — managed by /wiki-ingest -->
