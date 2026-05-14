# On the Convergence Rate of LoRA Gradient Descent

*paper, 2025. Siqiao Mu, Diego Klabjan. ICML 2026.*

First non-asymptotic convergence proof for practical LoRA GD without Lipschitz smoothness: O(1/log T) rate to a stationary point. Key technique is outer-product reparametrization of stacked adapter matrices plus a modified descent lemma. The slow rate and bilinear non-smoothness suggest that under high-variance RL gradients, convergence to low-rank degenerate stationary points is plausible.

→ [raw entry](../../raw/paper/lora-convergence-rate-gd/README.md) · [url](https://arxiv.org/abs/2512.18248)
