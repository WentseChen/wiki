---
title: "On the Convergence Rate of LoRA Gradient Descent"
url: https://arxiv.org/abs/2512.18248
type: paper
authors: [Siqiao Mu, Diego Klabjan]
venue: ICML 2026
year: 2025
topics: [theory, ml]
added: 2026-05-14
arxiv_id: 2512.18248
---

# On the Convergence Rate of LoRA Gradient Descent

**Link:** https://arxiv.org/abs/2512.18248

## Summary

This ICML 2026 paper delivers the first non-asymptotic convergence rate for the original LoRA gradient descent algorithm without restrictive assumptions (no Lipschitz smoothness, no artificial boundedness). The key challenge is that the LoRA objective — a product of two low-rank matrices — lacks the Lipschitz smoothness that standard convergence proofs require. The authors overcome this by reparametrizing the objective as the outer product of stacked adapter matrices and deriving a modified descent lemma tailored to the reformulated function, then controlling the step size to bound the gradient updates.

The main result proves convergence to a stationary point at rate O(1/log T), establishing the first rigorous non-asymptotic guarantee for LoRA as it is actually used in practice.

## Key points

- First non-asymptotic convergence analysis of practical LoRA GD, without Lipschitz smoothness or boundedness assumptions.
- Main result: O(1/log T) convergence to a stationary point — the logarithmic factor reflects the non-smooth structure of the LoRA bilinear factorization.
- Key technique: outer-product reparametrization of stacked adapter matrices + modified descent lemma for non-Lipschitz objectives.
- Step-size control (not Lipschitz smoothness) is the key mechanism enabling the proof.
- Directly relevant to rank collapse: the slow O(1/log T) rate and bilinear non-smoothness suggest that under high-variance RL gradients, convergence to degenerate (low-rank) stationary points is plausible.

## See also
- [[lora-convergence-implicit-bias]] — landscape analysis of LoRA stationary points
- [[lora-ntk-no-spurious-minima]] — NTK regime convergence guarantees
- [[lora-one-singular-subspace]] — linear convergence via gradient-aligned initialization
