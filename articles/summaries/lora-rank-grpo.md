# Gradient-Based LoRA Rank Allocation Under GRPO: An Empirical Study

*paper, 2026. Yash Ganpat Sawant.*

Empirical study showing that gradient-importance-based adaptive LoRA rank allocation — effective under SFT — fails under GRPO-based RL fine-tuning. The RL gradient landscape is far flatter (2.17x layer importance spread vs. >10x in SFT), causing proportional rank allocation to lose 4.5% accuracy versus uniform allocation. Directly supports the hypothesis that RL fine-tuning induces rank degeneracy pressures distinct from supervised training.

→ [raw entry](../../raw/paper/lora-rank-grpo/README.md) · [url](https://arxiv.org/abs/2605.07366)
