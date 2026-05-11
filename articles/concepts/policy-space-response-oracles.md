# Policy Space Response Oracles (PSRO)

Iterative multiagent-RL algorithm: maintain a growing population of policies, compute a meta-strategy (empirical-game equilibrium) over them, then train a new approximate best response against that meta-strategy and add it to the population. Generalizes fictitious play, double oracle, and self-play.

## Sources
- [[unified-game-theoretic-marl]]
