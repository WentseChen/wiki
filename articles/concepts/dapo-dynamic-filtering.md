# Dapo Dynamic Filtering

Dynamic sampling/filtering of rollouts using 0/1 reward scores to focus updates on informative trajectories. Originally introduced in DAPO; filters prompts whose group rollouts all share the same reward (all-correct or all-wrong), preserving gradient signal under group-relative advantage and mitigating entropy collapse.

## Sources
- [[openrlhf]]
- [[dapo-open-source-rl-system]]
