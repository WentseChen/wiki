# Intrinsic Dimensionality Explains the Effectiveness of Language Model Fine-Tuning

*paper, 2021. Armen Aghajanyan, Luke Zettlemoyer, Sonal Gupta. ACL 2021.*

Foundational paper showing pretrained LMs have very low intrinsic dimensionality: ~200 parameters in a random subspace suffice for 90% of full fine-tuning performance. Pre-training implicitly minimizes intrinsic dimension; larger models are lower-dimensional. Provides compression-based generalization bounds independent of full parameter count — the theoretical bedrock for LoRA and PEFT.

→ [raw entry](../../raw/paper/intrinsic-dim-lm-finetuning/README.md) · [url](https://arxiv.org/abs/2012.13255)
