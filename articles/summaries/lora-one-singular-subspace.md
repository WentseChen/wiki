# LoRA-One: One-Step Full Gradient Could Suffice for Fine-Tuning Large Language Models, Provably and Efficiently

*paper, 2025. Yuanhe Zhang, Fanghui Liu, Yudong Chen. ICML 2025 (Oral).*

Proves LoRA adapters align to the singular subspaces of the one-step full fine-tuning gradient under gradient descent. LoRA-One initializes from this gradient for immediate subspace alignment and linear convergence. Directly explains rank collapse: if the gradient's dominant singular subspace is low-rank (as under sparse RL rewards), the adapters collapse with it.

→ [raw entry](../../raw/paper/lora-one-singular-subspace/README.md) · [url](https://arxiv.org/abs/2502.01235)
