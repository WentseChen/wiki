# plasticity injection

Replacing a hidden layer `f(x)` with `f(x) + g(x) − g_frozen(x)`, where `g` is a freshly initialized copy of `f`. The output is unchanged at injection time but the network gains new trainable capacity — doubling as both a fix and a causal diagnostic for plasticity bottlenecks.

## Sources
- [[plasticity-injection-drl]]
