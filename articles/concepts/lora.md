# LoRA

Low-Rank Adaptation — parameter-efficient fine-tuning method that injects trainable low-rank matrices (A, B) into frozen pretrained weight layers, so only rank-r perturbations are learned instead of full weight updates.

## Sources
- [[fedlora-rank-collapse-prevention]]
- [[lora-convergence-rate-gd]]
- [[lora-one-singular-subspace]]
- [[intrinsic-dim-lm-finetuning]]
- [[lora-ntk-no-spurious-minima]]
- [[lora-convergence-implicit-bias]]
- [[lora-rank-grpo]]
- [[lora-vs-full-finetuning-illusion]]
- [[lora-spectral-geometry-training-objective]]
- [[lora-learns-less-forgets-less]]
- [[lora-rank-tradeoffs-knowledge-robustness]]
- [[essa-evolutionary-strategies-alignment]]
- [[goat-lora-adaptive-svd-moe]]
- [[lora-rlhf-efficiency-regularization]]
- [[pe-rlhf-parameter-efficient]]
- [[up-rlhf-diverse-lora-ensembles]]
- [[peft-preference-alignment-tradeoffs]]
- [[shared-lora-personalized-rlhf]]
- [[remix-rl-routing-mixture-loras]]
- [[molf-lora-full-finetuning-routing]]
- [[dapo-open-source-rl-system]]
- [[aepo-arbitrary-entropy-policy-optimization]]

## Interdisciplinary Notes
- In **NLP fine-tuning** ([[nlp]]), LoRA is treated as a near-drop-in for full FT — empirically validated for RLHF (per [[lora-rlhf-efficiency-regularization]], [[pe-rlhf-parameter-efficient]]) — but is geometrically distinct: it inserts "intruder dimensions" not present in full FT (per [[lora-vs-full-finetuning-illusion]]) and learns 10–100x lower effective rank deltas (per [[lora-learns-less-forgets-less]]).
- In **optimization theory** ([[theory]]), LoRA's stationary points are provably either low-rank global minima (the typical case under zero-init + weight decay) or high-rank spurious local minima (per [[lora-convergence-implicit-bias]]); rank ≳ √N suffices for no spurious minima in the NTK regime (per [[lora-ntk-no-spurious-minima]]); LoRA's first-order direction equals the dominant singular subspace of the one-step full-FT gradient (per [[lora-one-singular-subspace]]).
- In **RL fine-tuning** ([[rl]]), the gradient landscape is 5× flatter under GRPO than SFT (per [[lora-rank-grpo]]), so gradient-based adaptive rank allocation fails (loses 4.5% accuracy) — the *upstream* cause is entropy collapse at the policy level (per [[dapo-open-source-rl-system]], [[aepo-arbitrary-entropy-policy-optimization]]) shrinking the effective-rank of the policy-gradient covariance. LoRA, already rank-bounded, has nowhere to hide.
