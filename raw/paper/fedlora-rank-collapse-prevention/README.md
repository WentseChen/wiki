---
title: "Preventing Rank Collapse in Federated Low-Rank Adaptation with Client Heterogeneity"
url: https://arxiv.org/abs/2602.13486
type: paper
authors: [Fei Wu, Jia Hu, Geyong Min, Shiqiang Wang]
year: 2026
topics: [theory, ml]
added: 2026-05-14
arxiv_id: 2602.13486
---

# Preventing Rank Collapse in Federated Low-Rank Adaptation with Client Heterogeneity

**Link:** https://arxiv.org/abs/2602.13486

## Summary

This paper identifies and formally analyzes "rank collapse" in federated LoRA (FedLoRA) when clients use heterogeneous ranks. When clients with different LoRA ranks submit updates and a rank-agnostic aggregation scheme is applied, the energy of the global update concentrates in the minimum shared rank — higher-rank components are suppressed geometrically over successive training rounds. The authors prove that this suppression follows a geometric rate determined by the mismatch between aggregation weights and rank-dependent client contributions.

The proposed fix, raFLoRA, decomposes local updates into rank partitions and aggregates each partition separately, weighted by the effective contribution of clients at each rank level. While the setting is federated learning (not RL fine-tuning), the theoretical analysis of rank collapse — as a geometric concentration effect from aggregation weight mismatches — is a formal mechanistic result directly applicable to any multi-source gradient aggregation with rank heterogeneity, including LoRA training under high-variance / sparse-reward RL (where mini-batches contribute rank-heterogeneous gradients).

## Key points

- Formally identifies rank collapse in federated LoRA: energy of global update concentrates in minimum shared rank at a geometric rate.
- Root cause: mismatch between rank-agnostic aggregation weights and rank-dependent client contributions — proved, not just observed.
- raFLoRA: rank-partitioned aggregation weights each rank-level separately by effective client contribution, preventing collapse.
- Theoretical analysis is general: the geometric suppression mechanism applies wherever heterogeneous-rank gradient updates are aggregated without rank-aware weighting.
- Fresh preprint (Feb 2026).

## See also
- [[lora-convergence-implicit-bias]] — implicit bias toward low-rank in standard LoRA training
- [[lora-rank-grpo]] — rank collapse under GRPO RL training
