# agents

Agentic systems, tool use, planning, multi-agent.

## Overview

<!-- short overview, maintained by LLM as the topic grows -->

## Key concepts

<!-- bullet list of [[concept-slug]] links into articles/concepts/ -->

## Recent

- [[marti]] — Centralized MAS interaction + distributed policy training over OpenRLHF; rule-based + LLM-generated rewards. *Zhang et al., 2026.*
- [[magrpo-llm-collaboration]] — Cooperative MARL formulation for LLM collaboration via group-relative advantages. *Liu et al., 2025.*
- [[stronger-mas]] — AT-GRPO fixes GRPO's prompt/turn assumptions in multi-agent settings; planning accuracy 14→96+%. *Zhao et al., 2025.*
- [[agentrl-multi-turn-multi-task]] — Multi-turn multi-task agentic RL with fully-async pipeline; cross-policy sampling + task-advantage normalization. *Zhang et al., 2025.*
- [[flexmarl-rollout-training-codesign]] — FlexMARL: rollout-training co-design for LLM-MARL infra; 7.3× speedup, 5.6× hardware utilization. *Jiang et al., 2026.*
- [[gptswarm]] — Language agents as optimizable graphs; RL/re-prompt edge optimization for self-improving swarms. *Zhuge et al., 2024.*
- [[orchestration-traces-rl]] — RL on LLM-MAS via orchestration traces (temporal interaction graphs); 84-paper curated pool. *Zhang, 2026.*
- [[parl-parallel-agent-rl]] — Parallel-agent RL with staged reward shaping + critical-steps metric; coordinates ~100 sub-agents. *Swarm Corp, 2026.*
- [[multi-agents-debate]] — Adversarial debate + judge mitigates Degeneration of Thoughts in single-agent self-reflection. *Liang et al., 2023.*
- [[agentgym-rl]] — ScalingInter-RL progressive horizon scaling; 7B matches GPT-4o on WebArena. *Xi et al., 2025.*
- [[agent-r1]] — Modular end-to-end RL framework for tool-using LLM agents; MDP extension for agent contexts. *Cheng et al., 2025.*
- [[verlog]] — Multi-turn RL for 400+ turn LLM agent tasks; dual-discounted GAE + per-turn async rollouts. *Chen et al., 2025.*
- [[rllm]] — Framework-agnostic agent-RL via @rllm.rollout decorator; small models beat 50× larger via RL. *rllm-org, 2025.*
- [[practitioners-guide-multi-turn-rl]] — Empirical study of multi-turn agentic RL design space (env / reward / policy); PPO vs RLOO. *Wang et al., 2025.*
- [[areal]] — Fully-async RL system for language reasoning; 2.77× speedup; 14+ algorithms; 1.5B–235B scale. *Fu et al., 2025.*
- [[llm-based-marl-survey]] — Early survey of LLM-based MARL; coordination, communication, human-in-the-loop as open challenges. *Sun et al., 2024.*
- [[agentic-rl-landscape-survey]] — 500+ paper survey; reframes LLM-RL from single-step MDP to extended POMDP. *Zhang et al., 2025.*
- [[agentic-rl-training-recipes]] — Survey/repo cataloging agentic-RL training schemes, infra, env taxonomy, reward design. *Chang et al., 2026.*
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
- [[unified-game-theoretic-marl]] — PSRO: best-response RL against an empirical-game meta-strategy; diagnoses multiagent overfitting via joint-policy correlation. *Lanctot et al., 2017.*

<!-- newest at top — managed by /wiki-ingest -->
