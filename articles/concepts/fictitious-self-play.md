# Fictitious self-play

Self-play scheme where the current policy is trained against a mixture of all (or a sampled subset of) historical policy snapshots, rather than only the latest opponent. Approximates fictitious play from game theory and avoids the strategy cycles that plain self-play falls into.

## Sources
- [[neural-fictitious-self-play]]
- [[alphastar-grandmaster]]
