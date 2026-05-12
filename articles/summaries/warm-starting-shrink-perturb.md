# On Warm-Starting Neural Network Training

*paper, 2020. Ash, Adams.*

Documents that warm-started training (continue from a converged checkpoint after adding new data) generalizes worse than from-scratch training, and proposes "shrink-and-perturb" — `w := λw + ε·noise` — as a near-free fix. The seminal supervised-side ancestor of continual backprop and the L2-Init / reset family.

→ [raw entry](../../raw/paper/warm-starting-shrink-perturb/README.md) · [url](https://arxiv.org/abs/1910.08475)
