# systems

ML systems, infra, serving, training stacks.

## Overview

<!-- short overview, maintained by LLM as the topic grows -->

## Key concepts

<!-- bullet list of [[concept-slug]] links into articles/concepts/ -->

## Recent

- [[dapo-open-source-rl-system]] — DAPO names entropy collapse as core GRPO failure; decoupled clip-higher + dynamic sampling restore exploration; 50 pts AIME 2024. *Yu et al., 2025.*
- [[marti]] — Centralized MAS interaction + distributed policy training over OpenRLHF; rule-based + LLM-generated rewards. *Zhang et al., 2026.*
- [[agentrl-multi-turn-multi-task]] — Multi-turn multi-task agentic RL with fully-async pipeline; cross-policy sampling + task-advantage normalization. *Zhang et al., 2025.*
- [[flexmarl-rollout-training-codesign]] — FlexMARL: rollout-training co-design for LLM-MARL infra; 7.3× speedup, 5.6× hardware utilization. *Jiang et al., 2026.*
- [[parl-parallel-agent-rl]] — Parallel-agent RL with staged reward shaping + critical-steps metric; coordinates ~100 sub-agents. *Swarm Corp, 2026.*
- [[agentgym-rl]] — ScalingInter-RL progressive horizon scaling; 7B matches GPT-4o on WebArena. *Xi et al., 2025.*
- [[verlog]] — Multi-turn RL for 400+ turn LLM agent tasks; dual-discounted GAE + per-turn async rollouts. *Chen et al., 2025.*
- [[rllm]] — Framework-agnostic agent-RL via @rllm.rollout decorator; small models beat 50× larger via RL. *rllm-org, 2025.*
- [[areal]] — Fully-async RL system for language reasoning; 2.77× speedup; 14+ algorithms; 1.5B–235B scale. *Fu et al., 2025.*
- [[openrlhf]] — Ray + vLLM RLHF; PPO / REINFORCE++ / GRPO / RLOO; sync/async/hybrid; MARTI's parent codebase. *OpenRLHF, 2024.*
- [[verl-hybridflow]] — Hybrid-controller RL post-training; FSDP/Megatron/vLLM integration; backbone for many agentic-RL frameworks. *ByteDance Seed et al., 2024.*
- [[agentic-rl-training-recipes]] — Survey/repo cataloging agentic-RL training schemes, infra, env taxonomy, reward design. *Chang et al., 2026.*
<!-- newest at top — managed by /wiki-ingest -->
