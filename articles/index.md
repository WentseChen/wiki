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
- [[openrlhf]] — Ray + vLLM RLHF; PPO / REINFORCE++ / GRPO / RLOO; sync/async/hybrid; MARTI's parent codebase. *OpenRLHF, 2024.*
- [[verl-hybridflow]] — Hybrid-controller RL post-training; FSDP/Megatron/vLLM integration; backbone for many agentic-RL frameworks. *ByteDance Seed et al., 2024.*
- [[llm-based-marl-survey]] — Early survey of LLM-based MARL; coordination, communication, human-in-the-loop as open challenges. *Sun et al., 2024.*
- [[agentic-rl-landscape-survey]] — 500+ paper survey; reframes LLM-RL from single-step MDP to extended POMDP. *Zhang et al., 2025.*
- [[agentic-rl-training-recipes]] — Survey/repo cataloging agentic-RL training schemes, infra, env taxonomy, reward design. *Chang et al., 2026.*

<!-- newest at top, cap 20 — managed by /wiki-ingest -->
