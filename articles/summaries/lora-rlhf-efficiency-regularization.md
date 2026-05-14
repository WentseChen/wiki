# Exploring the impact of low-rank adaptation on the performance, efficiency, and regularization of RLHF

*paper, 2023. Sun, Gupta, Iyyer (UMass Amherst).*

Foundational LoRA+PPO paper showing LLaMA 7B can be RLHF-aligned on 2 A100s using 0.2% of parameters, outperforming the full AlpacaFarm checkpoint. Key finding: LoRA's low-rank constraint acts as an implicit regularizer, making KL penalty unnecessary and mitigating PPO-induced factuality degradation.

→ [raw entry](../../raw/paper/lora-rlhf-efficiency-regularization/README.md) · [url](https://arxiv.org/abs/2309.09055)
