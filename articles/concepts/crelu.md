# CReLU

Concatenated ReLU: an activation that outputs `[ReLU(x), ReLU(-x)]`, doubling the channel width while keeping both signs of the pre-activation. Drastically reduces dying-unit problems and mitigates plasticity loss in continual deep RL.

## Sources
- [[plasticity-loss-continual-drl]]
