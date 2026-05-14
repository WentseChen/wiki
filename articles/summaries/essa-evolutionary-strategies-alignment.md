# ESSA: Evolutionary Strategies for Scalable Alignment

*paper, 2025. Korotyshova et al.*

Gradient-free LLM alignment via evolutionary search over LoRA adapter singular values. By treating only the SVD singular values as optimization targets, ESSA avoids backpropagation entirely, works in INT4/INT8 quantized mode, and matches GRPO on math/instruction benchmarks. Implicitly demonstrates singular values encode the bulk of alignment information in LoRA weight space.

→ [raw entry](../../raw/paper/essa-evolutionary-strategies-alignment/README.md) · [url](https://arxiv.org/abs/2507.04453)
