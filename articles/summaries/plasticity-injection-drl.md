# Deep Reinforcement Learning with Plasticity Injection

*paper, 2023. Nikishin, Oh, Ostrovski, Lyle, Pascanu, Dabney, Barreto.*

Adds a zero-initialized residual branch `f(x) → f(x) + g(x) − g_frozen(x)` that leaves the network's output unchanged at injection time but adds fresh trainable capacity. Doubles as a causal diagnostic — does injection help? — for whether plasticity is the bottleneck. NeurIPS 2023 spotlight.

→ [raw entry](../../raw/paper/plasticity-injection-drl/README.md) · [url](https://arxiv.org/abs/2305.15555)
