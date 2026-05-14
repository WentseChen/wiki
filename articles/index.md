# Wiki index

Master entry point. Browse by topic, or scan recent additions below.

## Topics

- [nlp](topics/nlp.md) — language models, training, alignment, prompting, evaluation
- [rl](topics/rl.md) — reinforcement learning
- [agents](topics/agents.md) — agentic systems, tool use, multi-agent
- [self-play](topics/self-play.md) — self-play training
- [game-theory](topics/game-theory.md) — game theory
- [multimodal](topics/multimodal.md) — VLMs, multimodal
- [vision](topics/vision.md) — computer vision
- [systems](topics/systems.md) — ML systems, infra
- [continuous-learning](topics/continuous-learning.md) — continual learning
- [theory](topics/theory.md) — learning theory
- [bandit](topics/bandit.md) — bandits
- [ml](topics/ml.md) — general ML
- [others](topics/others.md) — misc

## Recent additions

- [[fedlora-rank-collapse-prevention]] — Proves rank-agnostic LoRA aggregation causes geometric energy concentration in min shared rank; raFLoRA fixes via rank-partitioned weighting. *Wu et al., 2026.*
- [[rmt-deep-learning-beyond-linear]] — High-dimensional Equivalent extends RMT to nonlinear deep nets; characterizes scaling laws, double descent, generalization; foundation for spectral rank analysis. *Liao & Mahoney, 2025 (IEEE SPM).*
- [[rmt-transformer-singular-values]] — RMT baseline reveals learned structure at both spectrum ends in transformers; small SVs carry information; fine-tuning shifts importance toward extremes. *Staats et al., 2024.*
- [[rank1-fisher-natural-policy-gradient]] — Rank-1 inverse-FIM approx for natural PG; proves faster convergence; low-rank FIM under sparse rewards grounds rank-collapse in RL. *Huo et al., 2026.*
- [[low-rank-bias-weight-decay-merging]] — Proves L2 weight decay induces parameter-gradient alignment + low-rank bias at GD stationary points; enables model merging via weight sum. *Kuzborskij & Abbasi Yadkori, 2025.*
- [[lora-convergence-rate-gd]] — First non-asymptotic LoRA GD convergence: O(1/log T) to stationary point without Lipschitz smoothness; outer-product reparametrization + modified descent lemma. *Mu & Klabjan, 2025 (ICML 2026).*
- [[lora-one-singular-subspace]] — Proves LoRA adapters align to singular subspaces of one-step full gradient; LoRA-One init achieves linear convergence; explains rank collapse. *Zhang et al., 2025 (ICML oral).*
- [[neural-collapse-low-rank-bias]] — L² weight decay jointly drives neural collapse and low-rank bias; proves distance to rank-K ∝ TCV/λ; benign landscape under regularization. *Zangrando et al., 2024.*
- [[intrinsic-dim-objective-landscapes]] — Defines intrinsic dimension via random-subspace training; shows RL/supervised problems have far smaller intrinsic dims than parameter counts; Pong ≈ CIFAR-10. *Li et al., 2018 (ICLR).*
- [[intrinsic-dim-lm-finetuning]] — Pretrained LMs have very low intrinsic dimensionality; ~200 params in random subspace achieves 90% of full FT; compression-based generalization bounds. *Aghajanyan et al., 2021 (ACL).*
- [[lora-ntk-no-spurious-minima]] — LoRA with rank ≳ √N eliminates all spurious local minima in NTK regime; gives data-size-dependent rank threshold. *Jang et al., 2024 (ICML).*
- [[lora-convergence-implicit-bias]] — Proves LoRA converges to low-rank global min or high-rank spurious min; implicit bias from zero-init + weight decay drives rank collapse. *Kim et al., 2025.*
- [[low-rank-pretraining-spectral-geometry]] — Low-rank pre-training converges to geometrically distinct solutions from full-rank even at matched perplexity; 16-metric spectral/geometric analysis. *Shivagunde et al., 2026.*
- [[molf-lora-full-finetuning-routing]] — MoLF routes gradient updates between LoRA and full FT at optimizer level; MoLF-Efficient routes among variable-rank LoRA experts. *Tang et al., 2026.*
- [[remix-rl-routing-mixture-loras]] — Routing collapse in Mixture-of-LoRAs fixed via RL gradient estimation on non-learnable routers; enforces balanced adapter utilization. *Qiu et al., 2026 (ICLR).*
- [[shared-lora-personalized-rlhf]] — LoRA in aggregated reward parameter space handles heterogeneous preferences; sample complexity guarantees for personalized RLHF. *Liu et al., 2025 (AISTATS).*
- [[peft-preference-alignment-tradeoffs]] — 300+ experiments: LoRA/QLoRA × SFT/DPO; SFT sometimes beats DPO; non-trivial PEFT-alignment interactions across model families. *Thakkar et al., 2024 (ACL).*
- [[up-rlhf-diverse-lora-ensembles]] — Diverse LoRA ensembles (nuclear norm diversity) quantify reward uncertainty; uncertainty penalty mitigates RLHF overoptimization. *Zhai et al., 2023.*
- [[pe-rlhf-parameter-efficient]] — LoRA-based PE-RLHF matches full RLHF on 6 tasks; 90% faster reward model training, 50% memory savings. *Sidahmed et al., 2024.*
- [[lora-rlhf-efficiency-regularization]] — LoRA-PPO aligns LLaMA 7B on 2 A100s (0.2% params); KL penalty unneeded (implicit regularization); mitigates PPO factuality degradation. *Sun et al., 2023.*
<!-- newest at top, cap 20 — managed by /wiki-ingest -->
