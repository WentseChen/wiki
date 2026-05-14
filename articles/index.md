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

- [[low-rank-pretraining-spectral-geometry]] — Low-rank pre-training converges to geometrically distinct solutions from full-rank even at matched perplexity; 16-metric spectral/geometric analysis. *Shivagunde et al., 2026.*
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
- [[lora-rank-grpo]] — Gradient-based rank allocation fails under GRPO: RL gradient landscape is 5× flatter than SFT, causing adaptive LoRA to lose 4.5% accuracy vs. uniform. *Sawant, 2026.*
- [[marti]] — Centralized MAS interaction + distributed policy training over OpenRLHF; rule-based + LLM-generated rewards. *Zhang et al., 2026.*
- [[magrpo-llm-collaboration]] — Cooperative MARL formulation for LLM collaboration via group-relative advantages. *Liu et al., 2025.*
- [[stronger-mas]] — AT-GRPO fixes GRPO's prompt/turn assumptions in multi-agent settings; planning accuracy 14→96+%. *Zhao et al., 2025.*
- [[agentrl-multi-turn-multi-task]] — Multi-turn multi-task agentic RL with fully-async pipeline; cross-policy sampling + task-advantage normalization. *Zhang et al., 2025.*
<!-- newest at top, cap 20 — managed by /wiki-ingest -->
