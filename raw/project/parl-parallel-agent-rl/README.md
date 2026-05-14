---
title: PARL: Parallel-Agent Reinforcement Learning
url: https://github.com/The-Swarm-Corporation/PARL
type: project
authors: [The Swarm Corporation]
venue: GitHub (Kimi K2.5 community impl)
year: 2026
topics: [agents, rl, systems]
added: 2026-05-13
github: The-Swarm-Corporation/PARL
---

# PARL: Parallel-Agent Reinforcement Learning

**Link:** https://github.com/The-Swarm-Corporation/PARL

## Summary
Trains an orchestrator LLM to decompose tasks into parallel sub-agent calls. Three-component reward (instantiation + finish + perf) with annealed coefficients, critical-path latency metric, and orchestrator–subagent architecture. Open re-implementation of Kimi K2.5's PARL.

## Key points
- Staged reward annealing: parallelism first, completion later
- 3-part reward: r_parallel + r_finish + r_perf
- Critical-steps latency metric (parallel critical path)
- Trainable orchestrator + frozen sub-agents
- Coordinates ~100 sub-agents over 1500+ steps

## See also
<!-- add [[related-slug]] links as connections form -->
