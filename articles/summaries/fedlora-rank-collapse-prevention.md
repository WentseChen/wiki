# Preventing Rank Collapse in Federated Low-Rank Adaptation with Client Heterogeneity

*paper, 2026. Fei Wu, Jia Hu, Geyong Min, Shiqiang Wang.*

Formally proves that rank-agnostic aggregation of heterogeneous-rank LoRA updates causes geometric concentration of gradient energy in the minimum shared rank — rank collapse. raFLoRA fixes this via rank-partitioned aggregation. The geometric suppression mechanism is general: it applies to any setting where rank-heterogeneous gradients are aggregated without rank-aware weighting, including sparse-reward RL.

→ [raw entry](../../raw/paper/fedlora-rank-collapse-prevention/README.md) · [url](https://arxiv.org/abs/2602.13486)
