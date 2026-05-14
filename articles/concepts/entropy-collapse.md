# Entropy Collapse

The monotonic decrease of policy entropy during RL fine-tuning of LLMs — particularly under group-relative policy optimization (GRPO, RLVR) — leading to near-deterministic, near-identical outputs within a group and the loss of exploration. Distinct from but mechanistically linked to weight-level rank collapse: as the policy concentrates probability mass on a few tokens at every step, the gradient signal shrinks to a low-dimensional subspace (advantage-weighted log-prob of dominant tokens), inducing low effective-rank updates in the parameter space.

## Sources
- [[dapo-open-source-rl-system]]
- [[aepo-arbitrary-entropy-policy-optimization]]
- [[lora-rank-grpo]]
- [[rank1-fisher-natural-policy-gradient]]
