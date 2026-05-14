# Grpo

Group Relative Policy Optimization — uses group-relative advantages over a sampled set of trajectories instead of a learned value function. Empirically suffers from entropy collapse (DAPO) and produces a far flatter gradient landscape than SFT (max-to-min layer importance 2.17x vs >10x), breaking gradient-based LoRA rank allocation heuristics.

## Sources
- [[magrpo-llm-collaboration]]
- [[stronger-mas]]
- [[lora-rank-grpo]]
- [[dapo-open-source-rl-system]]
