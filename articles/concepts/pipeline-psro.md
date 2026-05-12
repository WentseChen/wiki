# Pipeline PSRO (P2SRO)

Parallel PSRO: a hierarchical pipeline of RL workers train concurrently, each best-responding to the meta-Nash of the levels below; the lowest worker becomes fixed once it plateaus, then a new active worker is appended. Preserves PSRO's convergence guarantees while scaling with parallel compute.

## Sources
- [[pipeline-psro]]
