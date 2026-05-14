# ml

General machine learning — supervised, self-supervised, other.

## Overview

<!-- short overview, maintained by LLM as the topic grows -->

## Key concepts

<!-- bullet list of [[concept-slug]] links into articles/concepts/ -->

## Recent

- [[low-rank-pretraining-spectral-geometry]] — Low-rank pre-training converges to geometrically distinct solutions from full-rank even at matched perplexity; 16-metric spectral/geometric analysis. *Shivagunde et al., 2026.*
- [[molf-lora-full-finetuning-routing]] — MoLF routes gradient updates between LoRA and full FT at optimizer level; MoLF-Efficient routes among variable-rank LoRA experts. *Tang et al., 2026.*
- [[goat-lora-adaptive-svd-moe]] — GOAT: SVD-structured MoE routes to relevant singular value priors; closes LoRA-vs-full-FT gap on 25 datasets. *Fan et al., 2025 (ICML).*
- [[lora-rank-tradeoffs-knowledge-robustness]] — LoRA rank has non-monotonic effect: past an optimum, higher rank accelerates forgetting with no in-domain gain; spectral analysis confirms. *Rathore et al., 2025 (AACL).*
- [[lora-learns-less-forgets-less]] — LoRA underperforms full FT on in-domain tasks; full FT learns 10–100x higher effective rank; LoRA forgets less but learns less. *Biderman et al., 2024 (TMLR).*
- [[lora-spectral-geometry-training-objective]] — Spectral features (effective rank, stable rank) of LoRA deltas classify training objective at AUC~1.00 and predict harmful compliance. *Paul, 2026.*
- [[lora-vs-full-finetuning-illusion]] — LoRA inserts "intruder dimensions" (anomalous high-rank singular vectors) that causally drive forgetting; LoRA ≠ full FT spectrally. *Shuttleworth et al., 2024.*
- [[lora-rank-grpo]] — Gradient-based rank allocation fails under GRPO: RL gradient landscape is 5× flatter than SFT, causing adaptive LoRA to lose 4.5% accuracy vs. uniform. *Sawant, 2026.*
- [[warm-starting-shrink-perturb]] — Continued training generalizes worse than from-scratch; shrink-and-perturb closes the gap. *Ash & Adams, 2020.*
- [[l2-init-regenerative]] — L2-regularize toward initial parameters (not zero) to preserve plasticity in continual supervised learning. *Kumar et al., 2023.*
- [[plasticity]] — Deep nets lose plasticity under continual training; continual backprop (reinit least-used units) restores it. *Dohare et al., 2024.*

<!-- newest at top — managed by /wiki-ingest -->
