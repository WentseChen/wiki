---
title: "ReMix: Reinforcement Routing for Mixtures of LoRAs in LLM Finetuning"
url: https://arxiv.org/abs/2603.10160
type: paper
authors: [Ruizhong Qiu, Hanqing Zeng, Yinglong Xia, Yiwen Meng, Ren Chen, Jiarui Feng, Dongqi Fu, Qifan Wang, Jiayi Liu, Jun Xiao, Xiangjun Fan, Benyu Zhang, Hong Li, Zhining Liu, Hyunsik Yoo, Zhichen Zeng, Tianxin Wei, Hanghang Tong]
venue: LLA @ ICLR 2026
year: 2026
topics: [rl, nlp]
added: 2026-05-14
arxiv_id: "2603.10160"
---

# ReMix: Reinforcement Routing for Mixtures of LoRAs in LLM Finetuning

**Link:** https://arxiv.org/abs/2603.10160

## Summary

ReMix identifies a routing collapse problem in Mixture-of-LoRAs systems: existing learnable routing weights become severely imbalanced, collapsing so that only one or two LoRA adapters dominate all routing probability. This is an instance of rank/capacity collapse at the router level — even if individual LoRA adapters have full rank, effective capacity collapses when most inputs route through a single adapter.

The proposed solution uses non-learnable routing weights with a reinforcement learning gradient estimator: since non-learnable weights cannot receive gradient-based updates, the loss is treated as a reward and RL techniques are applied to optimize a discrete routing policy. This enforces balanced adapter utilization across the mixture. Results show ReMix significantly outperforms state-of-the-art PEFT methods on multiple benchmarks.

## Key points

- Routing collapse in Mixture-of-LoRAs: learnable routers concentrate on 1-2 adapters, wasting ensemble capacity.
- Non-learnable routing weights prevent gradient-based collapse; RL gradient estimation enables optimization.
- Treating the training loss as a reward signal allows discrete routing policy optimization.
- Directly applicable to the LoRA+RL intersection: RL is used to fix a capacity collapse caused by learned routing.
- Published at LLA @ ICLR 2026.

## See also
<!-- [[goat-lora-adaptive-svd-moe]] [[lora-rank-grpo]] -->
