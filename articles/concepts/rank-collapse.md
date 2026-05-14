# rank collapse

Progressive reduction of the effective rank of a network's learned features (or weight matrices) over training. In deep RL, induced by iterated bootstrapped regression onto self-generated targets.

## Sources
- [[fedlora-rank-collapse-prevention]]
- [[implicit-under-parameterization]]
- [[remix-rl-routing-mixture-loras]]
- [[lora-rank-grpo]]
- [[lora-vs-full-finetuning-illusion]]
- [[neural-collapse-low-rank-bias]]
- [[low-rank-bias-weight-decay-merging]]
- [[lora-convergence-implicit-bias]]
- [[rank1-fisher-natural-policy-gradient]]
- [[capacity-loss-rl]]

## Interdisciplinary Notes
- In **deep RL** ([[rl]]), rank collapse is empirically attributed to bootstrapped value regression onto non-stationary self-generated targets — Kumar et al.'s "implicit under-parameterization" (per [[implicit-under-parameterization]]) and Lyle et al.'s "capacity loss" (per [[capacity-loss-rl]]) frame it as a degenerate response of TD-style learning to its own moving target. Empirical correlates: shrinking feature rank, weight-norm explosion, dead units (per [[plasticity]], [[plasticity-loss-continual-drl]]).
- In **optimization theory** ([[theory]], [[ml]]), the same phenomenon is the *implicit bias* of L2-regularized gradient descent: weight decay provably drives stationary points to low rank (per [[low-rank-bias-weight-decay-merging]]) and jointly induces neural collapse (per [[neural-collapse-low-rank-bias]]), independent of any RL signal.
- In **LoRA / PEFT** ([[nlp]], [[ml]]), the bias compounds: LoRA *starts* rank-bounded, then zero-init + weight decay produce an additional implicit bias toward low-rank, small-magnitude global minima (per [[lora-convergence-implicit-bias]]); LoRA adapters align to dominant singular subspaces of the one-step full gradient (per [[lora-one-singular-subspace]]). Under RL, if that gradient subspace is itself rank-degenerate (sparse rewards, low-rank Fisher per [[rank1-fisher-natural-policy-gradient]]), LoRA collapses to it.
- In **federated/multi-source training**, rank collapse is purely an aggregation artifact: heterogeneous-rank client updates with rank-agnostic averaging geometrically concentrate energy in the minimum shared rank (per [[fedlora-rank-collapse-prevention]]) — same effect, no neural network needed.
