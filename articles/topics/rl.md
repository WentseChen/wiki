# rl

Reinforcement learning — policy/value methods, exploration, offline RL.

## Overview

<!-- short overview, maintained by LLM as the topic grows -->

## Key concepts

<!-- bullet list of [[concept-slug]] links into articles/concepts/ -->

## Recent

- [[aepo-arbitrary-entropy-policy-optimization]] — AEPO reformulates entropy regulation as a PG problem via REINFORCE on temperature-adjusted samples; avoids reward-vs-entropy trade-off; dual of weight-side rank collapse. *Wang et al., 2025.*
- [[dapo-open-source-rl-system]] — DAPO names entropy collapse as core GRPO failure; decoupled clip-higher + dynamic sampling restore exploration; 50 pts AIME 2024 on Qwen2.5-32B. *Yu et al., 2025.*
- [[rank1-fisher-natural-policy-gradient]] — Rank-1 inverse-FIM approx for scalable natural PG; proves faster convergence; low-rank FIM under sparse rewards grounds rank-collapse in RL. *Huo et al., 2026.*
- [[intrinsic-dim-objective-landscapes]] — Defines intrinsic dimension via random-subspace training; shows RL/supervised problems have far smaller intrinsic dims than parameter counts; Pong ≈ CIFAR-10 difficulty. *Li et al., 2018 (ICLR).*
- [[remix-rl-routing-mixture-loras]] — Routing collapse in Mixture-of-LoRAs fixed via RL gradient estimation on non-learnable routers; enforces balanced adapter utilization. *Qiu et al., 2026 (ICLR).*
- [[shared-lora-personalized-rlhf]] — LoRA in aggregated reward parameter space handles heterogeneous preferences; sample complexity guarantees for personalized RLHF. *Liu et al., 2025 (AISTATS).*
- [[peft-preference-alignment-tradeoffs]] — 300+ experiments: LoRA/QLoRA × SFT/DPO; SFT sometimes beats DPO; non-trivial PEFT-alignment interactions across model families. *Thakkar et al., 2024 (ACL).*
- [[up-rlhf-diverse-lora-ensembles]] — Diverse LoRA ensembles (nuclear norm diversity) quantify reward uncertainty; uncertainty penalty mitigates RLHF overoptimization. *Zhai et al., 2023.*
- [[pe-rlhf-parameter-efficient]] — LoRA-based PE-RLHF matches full RLHF on 6 tasks; 90% faster reward model training, 50% memory savings. *Sidahmed et al., 2024.*
- [[lora-rlhf-efficiency-regularization]] — LoRA-PPO aligns LLaMA 7B on 2 A100s (0.2% params); KL penalty unneeded (implicit regularization); mitigates PPO factuality degradation. *Sun et al., 2023.*
- [[essa-evolutionary-strategies-alignment]] — Gradient-free alignment via evolutionary search over LoRA singular values; matches GRPO without backprop; shows SVs encode alignment info. *Korotyshova et al., 2025.*
- [[rl-vs-sft-singular-vector-analysis]] — RL fine-tuning corrects SFT-induced singular-vector drift; direction changes dominate magnitude; top-20% SVD directions recover 70-80% OOD perf. *Jin et al., 2025.*
- [[lora-rank-grpo]] — Gradient-based rank allocation fails under GRPO: RL gradient landscape is 5× flatter than SFT, causing adaptive LoRA to lose 4.5% accuracy vs. uniform. *Sawant, 2026.*
- [[marti]] — Centralized MAS interaction + distributed policy training over OpenRLHF; rule-based + LLM-generated rewards. *Zhang et al., 2026.*
- [[magrpo-llm-collaboration]] — Cooperative MARL formulation for LLM collaboration via group-relative advantages. *Liu et al., 2025.*
- [[stronger-mas]] — AT-GRPO fixes GRPO's prompt/turn assumptions in multi-agent settings; planning accuracy 14→96+%. *Zhao et al., 2025.*
- [[agentrl-multi-turn-multi-task]] — Multi-turn multi-task agentic RL with fully-async pipeline; cross-policy sampling + task-advantage normalization. *Zhang et al., 2025.*
- [[flexmarl-rollout-training-codesign]] — FlexMARL: rollout-training co-design for LLM-MARL infra; 7.3× speedup, 5.6× hardware utilization. *Jiang et al., 2026.*
- [[gptswarm]] — Language agents as optimizable graphs; RL/re-prompt edge optimization for self-improving swarms. *Zhuge et al., 2024.*
- [[orchestration-traces-rl]] — RL on LLM-MAS via orchestration traces (temporal interaction graphs); 84-paper curated pool. *Zhang, 2026.*
- [[parl-parallel-agent-rl]] — Parallel-agent RL with staged reward shaping + critical-steps metric; coordinates ~100 sub-agents. *Swarm Corp, 2026.*
- [[agentgym-rl]] — ScalingInter-RL progressive horizon scaling; 7B matches GPT-4o on WebArena. *Xi et al., 2025.*
- [[agent-r1]] — Modular end-to-end RL framework for tool-using LLM agents; MDP extension for agent contexts. *Cheng et al., 2025.*
- [[verlog]] — Multi-turn RL for 400+ turn LLM agent tasks; dual-discounted GAE + per-turn async rollouts. *Chen et al., 2025.*
- [[rllm]] — Framework-agnostic agent-RL via @rllm.rollout decorator; small models beat 50× larger via RL. *rllm-org, 2025.*
- [[practitioners-guide-multi-turn-rl]] — Empirical study of multi-turn agentic RL design space (env / reward / policy); PPO vs RLOO. *Wang et al., 2025.*
- [[areal]] — Fully-async RL system for language reasoning; 2.77× speedup; 14+ algorithms; 1.5B–235B scale. *Fu et al., 2025.*
- [[openrlhf]] — Ray + vLLM RLHF; PPO / REINFORCE++ / GRPO / RLOO; sync/async/hybrid; MARTI's parent codebase. *OpenRLHF, 2024.*
- [[verl-hybridflow]] — Hybrid-controller RL post-training; FSDP/Megatron/vLLM integration; backbone for many agentic-RL frameworks. *ByteDance Seed et al., 2024.*
- [[llm-based-marl-survey]] — Early survey of LLM-based MARL; coordination, communication, human-in-the-loop as open challenges. *Sun et al., 2024.*
- [[agentic-rl-landscape-survey]] — 500+ paper survey; reframes LLM-RL from single-step MDP to extended POMDP. *Zhang et al., 2025.*
- [[agentic-rl-training-recipes]] — Survey/repo cataloging agentic-RL training schemes, infra, env taxonomy, reward design. *Chang et al., 2026.*
- [[primacy-bias-deep-rl]] — Periodic resets of the last few layers cure deep RL's overfitting to early data and unlock high replay ratios. *Nikishin et al., 2022.*
- [[dormant-neuron-phenomenon]] — Hidden units go "dormant" during DQN training; ReDo periodically reinitializes them to restore capacity. *Sokar et al., 2023.*
- [[capacity-loss-rl]] — Non-stationary TD targets shrink feature rank; InFeR regularizes features toward init to preserve capacity. *Lyle et al., 2022.*
- [[implicit-under-parameterization]] — Bootstrapped value learning collapses the feature matrix to low effective rank in deep RL. *Kumar et al., 2021.*
- [[plasticity-loss-continual-drl]] — Plasticity loss clearly demonstrated on continual Atari; CReLU activations largely mitigate it. *Abbas et al., 2023.*
- [[understanding-plasticity-nn]] — Plasticity loss is driven by loss-landscape curvature blowup; dead units are downstream symptoms. *Lyle et al., 2023.*
- [[plasticity-injection-drl]] — Zero-impact residual injection adds trainable capacity and serves as a causal plasticity diagnostic. *Nikishin et al., 2023.*
- [[plasticity]] — Deep nets lose plasticity under continual training; continual backprop (reinit least-used units) restores it. *Dohare et al., 2024.*
- [[diayn-skill-discovery]] — Unsupervised skill discovery via MI between latent skill and visited states. *Eysenbach et al., 2019.*
- [[dvd-population-diversity]] — Population diversity as determinant of kernel over behavioral embeddings. *Parker-Holder et al., 2020.*
- [[smerl-structured-maxent-rl]] — Multiple near-optimal solutions in one MDP via latent-gated diversity bonus. *Kumar et al., 2020.*
- [[diverse-successor-features]] — CMDP framing of diverse-near-optimal RL with SF-correlation diversity. *Zahavy et al., 2021.*
- [[domino-diversity-near-optimality]] — CMDP framing of diverse RL using state-occupancy distance. *Zahavy et al., 2022.*
- [[novelty-search-abandoning-objectives]] — Pure-novelty search beats objective-based search on deceptive tasks. *Lehman & Stanley, 2011.*
- [[map-elites]] — QD algorithm filling a discretized behavior-space archive with elites. *Mouret & Clune, 2015.*
- [[dads-dynamics-aware-skills]] — Unsupervised skills that are both diverse and predictable, enabling latent-space MPC. *Sharma et al., 2020.*
- [[icm-curiosity-driven-exploration]] — Curiosity = forward-model error in inverse-model feature space. *Pathak et al., 2017.*
- [[alphastar-grandmaster]] — Grandmaster SC2 via league training (mains + exploiters) over self-play. *Vinyals et al., 2019.*
- [[reward-switching-policy-optimization]] — Iteratively discovers diverse policies by switching extrinsic/intrinsic reward on trajectory novelty. *Zhou et al., 2022.*
- [[neupl-neural-population-learning]] — One conditional net represents the whole PSRO population, all policies trained concurrently. *Liu et al., 2022.*
- [[anytime-psro]] — APSRO picks a meta-distribution that monotonically decreases exploitability vs the full game. *McAleer et al., 2022.*
- [[jpsro-correlated-equilibrium]] — JPSRO uses (C)CE meta-solvers + MGCE selection; extends PSRO to n-player general-sum games. *Marris et al., 2021.*
- [[diverse-psro-behavioural-diversity]] — Diverse PSRO with a DPP diversity kernel; lower exploitability on open-ended games. *Perez-Nieves et al., 2021.*
- [[xdo-extensive-form-double-oracle]] — Mixes best responses at every infostate; linear-in-infostates Nash convergence. *McAleer et al., 2021.*
- [[pipeline-psro]] — Parallel PSRO via hierarchical RL workers; SOTA on Barrage Stratego with guarantees preserved. *McAleer et al., 2020.*
- [[alpha-psro-generalized-training]] — α-PSRO: uses α-Rank as meta-solver, extending PSRO to general-sum many-player games. *Muller et al., 2020.*
- [[alpha-rank]] — Markov-Conley-chain ranking; unique, polynomial-time, drop-in PSRO meta-solver. *Omidshafiei et al., 2019.*
- [[open-ended-learning-symmetric-zero-sum]] — Rectified Nash Response: niching best-response for nontransitive games. *Balduzzi et al., 2019.*
- [[neural-fictitious-self-play]] — NFSP: deep-RL fictitious play, first scalable Nash solver for imperfect-info games. *Heinrich & Silver, 2016.*
- [[unified-game-theoretic-marl]] — PSRO: best-response RL against an empirical-game meta-strategy; diagnoses multiagent overfitting via joint-policy correlation. *Lanctot et al., 2017.*

<!-- newest at top — managed by /wiki-ingest -->
