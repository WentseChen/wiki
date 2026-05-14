# ml

General machine learning — supervised, self-supervised, other.

## Overview

<!-- short overview, maintained by LLM as the topic grows -->

## Key concepts

<!-- bullet list of [[concept-slug]] links into articles/concepts/ -->

## Recent

- [[fedlora-rank-collapse-prevention]] — Proves rank-agnostic aggregation of heterogeneous-rank LoRA updates causes geometric energy concentration in min shared rank; raFLoRA fixes via rank-partitioned weighting. *Wu et al., 2026.*
- [[rmt-deep-learning-beyond-linear]] — High-dimensional Equivalent extends RMT to nonlinear deep nets; characterizes scaling laws, double descent, generalization; foundation for spectral rank analysis. *Liao & Mahoney, 2025 (IEEE SPM).*
- [[low-rank-bias-weight-decay-merging]] — Proves L2 weight decay induces parameter-gradient alignment + low-rank bias at stationary points; enables model merging via weight sum under orthogonal inputs. *Kuzborskij & Abbasi Yadkori, 2025.*
- [[lora-convergence-rate-gd]] — First non-asymptotic LoRA GD convergence: O(1/log T) to stationary point without Lipschitz smoothness; outer-product reparametrization + modified descent lemma. *Mu & Klabjan, 2025 (ICML 2026).*
- [[neural-collapse-low-rank-bias]] — L² weight decay jointly drives neural collapse and low-rank bias; proves distance to rank-K ∝ TCV/λ; benign landscape under regularization. *Zangrando et al., 2024.*
- [[lora-ntk-no-spurious-minima]] — LoRA with rank ≳ √N eliminates all spurious local minima in NTK regime; gives data-size-dependent rank threshold. *Jang et al., 2024 (ICML).*
- [[lora-convergence-implicit-bias]] — Proves LoRA converges to low-rank global min or high-rank spurious min; implicit bias from zero-init + weight decay drives rank collapse. *Kim et al., 2025.*
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
