# ReMix: Reinforcement Routing for Mixtures of LoRAs in LLM Finetuning

*paper, 2026. Qiu et al. LLA @ ICLR 2026.*

Identifies routing collapse in Mixture-of-LoRAs (learnable routers concentrate on 1-2 adapters, wasting capacity) and fixes it with non-learnable routing optimized via RL gradient estimation — treating loss as reward. A direct example of RL solving a LoRA capacity collapse problem; outperforms SOTA PEFT methods.

→ [raw entry](../../raw/paper/remix-rl-routing-mixture-loras/README.md) · [url](https://arxiv.org/abs/2603.10160)
