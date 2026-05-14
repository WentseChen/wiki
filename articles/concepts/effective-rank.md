# Effective Rank

A soft measure of the number of significant dimensions in a matrix, computed from the entropy of the normalized singular value distribution (Roy & Vetterli, 2007). Full fine-tuning produces weight perturbations with 10–100x higher effective rank than typical LoRA configurations, suggesting LoRA imposes a genuine capacity bottleneck.

## Sources
- [[lora-learns-less-forgets-less]]
- [[lora-rank-grpo]]
- [[lora-spectral-geometry-training-objective]]
- [[lora-rank-tradeoffs-knowledge-robustness]]
- [[molf-lora-full-finetuning-routing]]
- [[capacity-loss-rl]]
- [[implicit-under-parameterization]]
- [[rmt-transformer-singular-values]]

## Interdisciplinary Notes
- In **NLP / PEFT** ([[nlp]]), effective rank is the diagnostic that distinguishes LoRA from full fine-tuning: full FT learns 10–100x higher effective rank perturbations than typical LoRA configs (per [[lora-learns-less-forgets-less]]), and the spectral geometry of LoRA deltas (effective rank, stable rank, SV entropy) classifies training objective at AUC ~1.00 (per [[lora-spectral-geometry-training-objective]]).
- In **RL theory** ([[rl]], [[theory]]), feature effective rank is the operational measure of "capacity loss" introduced by Lyle et al. (per [[capacity-loss-rl]]) and earlier "implicit under-parameterization" by Kumar et al. (per [[implicit-under-parameterization]]) — bootstrapped TD learning provably shrinks it.
- In **random matrix theory** ([[theory]]), the same quantity is interpreted as deviation from the Marchenko-Pastur baseline: the smallest decile of singular values carries third-most influence on perplexity post-FT (per [[rmt-transformer-singular-values]]), so effective rank loss in *either* tail is informationally costly — not just the top.
