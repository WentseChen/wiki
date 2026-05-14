# theory

Learning theory, optimization, generalization.

## Overview

<!-- short overview, maintained by LLM as the topic grows -->

## Key concepts

<!-- bullet list of [[concept-slug]] links into articles/concepts/ -->

## Recent

- [[fedlora-rank-collapse-prevention]] — Proves rank-agnostic aggregation of heterogeneous-rank LoRA updates causes geometric energy concentration in min shared rank; raFLoRA fixes via rank-partitioned weighting. *Wu et al., 2026.*
- [[rmt-deep-learning-beyond-linear]] — High-dimensional Equivalent extends RMT to nonlinear deep nets; characterizes scaling laws, double descent, generalization; foundation for spectral rank analysis. *Liao & Mahoney, 2025 (IEEE SPM).*
- [[rmt-transformer-singular-values]] — RMT baseline (Marchenko-Pastur) reveals learned structure at both spectrum ends in transformers; small SVs matter; fine-tuning shifts importance toward extremes. *Staats et al., 2024.*
- [[rank1-fisher-natural-policy-gradient]] — Rank-1 inverse-FIM approx for scalable natural PG; proves faster convergence; low-rank FIM under sparse rewards grounds rank-collapse in RL. *Huo et al., 2026.*
- [[low-rank-bias-weight-decay-merging]] — Proves L2 weight decay induces parameter-gradient alignment + low-rank bias at stationary points; enables model merging via weight sum under orthogonal inputs. *Kuzborskij & Abbasi Yadkori, 2025.*
- [[lora-convergence-rate-gd]] — First non-asymptotic LoRA GD convergence: O(1/log T) to stationary point without Lipschitz smoothness; outer-product reparametrization + modified descent lemma. *Mu & Klabjan, 2025 (ICML 2026).*
- [[lora-one-singular-subspace]] — Proves LoRA adapters align to singular subspaces of one-step full gradient; LoRA-One init achieves linear convergence; explains rank collapse under sparse-reward RL. *Zhang et al., 2025 (ICML oral).*
- [[neural-collapse-low-rank-bias]] — L² weight decay jointly drives neural collapse and low-rank bias; proves distance to rank-K ∝ TCV/λ; benign landscape under regularization. *Zangrando et al., 2024.*
- [[intrinsic-dim-objective-landscapes]] — Defines intrinsic dimension via random-subspace training; shows RL/supervised problems have far smaller intrinsic dims than parameter counts; Pong ≈ CIFAR-10 difficulty. *Li et al., 2018 (ICLR).*
- [[intrinsic-dim-lm-finetuning]] — Pretrained LMs have very low intrinsic dimensionality; ~200 params in random subspace achieves 90% of full FT; compression-based generalization bounds. *Aghajanyan et al., 2021 (ACL).*
- [[lora-ntk-no-spurious-minima]] — LoRA with rank ≳ √N eliminates all spurious local minima in NTK regime; gives data-size-dependent rank threshold. *Jang et al., 2024 (ICML).*
- [[lora-convergence-implicit-bias]] — Proves LoRA converges to low-rank global min or high-rank spurious min; implicit bias from zero-init + weight decay drives rank collapse. *Kim et al., 2025.*
- [[low-rank-pretraining-spectral-geometry]] — Low-rank pre-training converges to geometrically distinct solutions from full-rank even at matched perplexity; 16-metric spectral/geometric analysis. *Shivagunde et al., 2026.*
- [[capacity-loss-rl]] — Non-stationary TD targets shrink feature rank; InFeR regularizes features toward init to preserve capacity. *Lyle et al., 2022.*
- [[implicit-under-parameterization]] — Bootstrapped value learning collapses the feature matrix to low effective rank in deep RL. *Kumar et al., 2021.*
- [[understanding-plasticity-nn]] — Plasticity loss is driven by loss-landscape curvature blowup; dead units are downstream symptoms. *Lyle et al., 2023.*
- [[ewc-elastic-weight-consolidation]] — Quadratic penalty around each task's weights (Fisher-weighted) overcomes catastrophic forgetting. *Kirkpatrick et al., 2017.*

<!-- newest at top — managed by /wiki-ingest -->
