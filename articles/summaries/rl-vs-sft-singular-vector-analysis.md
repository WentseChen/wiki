# RL Is Neither a Panacea Nor a Mirage: Understanding Supervised vs. Reinforcement Learning Fine-Tuning for LLMs

*paper, 2025. Jin, Lv, Wu, Hamdaqa.*

Spectral study showing RL fine-tuning primarily corrects SFT-induced singular-vector drift rather than acquiring new capacity. Singular vector direction shifts (not magnitude) drive OOD recovery; restoring top-20% singular value directions recovers 70-80% of OOD performance. Relevant to understanding why RL gradients interact differently with low-rank subspaces than SFT gradients.

→ [raw entry](../../raw/paper/rl-vs-sft-singular-vector-analysis/README.md) · [url](https://arxiv.org/abs/2508.16546)
