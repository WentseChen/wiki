# Beyond LoRA vs. Full Fine-Tuning: Gradient-Guided Optimizer Routing for LLM Adaptation

*paper, 2026. Tang et al.*

MoLF dynamically routes gradient updates between LoRA and full fine-tuning at the optimizer level, guided by per-layer gradient statistics. Directly addresses the documented LoRA underperformance gap. MoLF-Efficient variant routes among LoRA experts of varying ranks for memory-constrained settings; outperforms prior adaptive rank methods including under RL fine-tuning.

→ [raw entry](../../raw/paper/molf-lora-full-finetuning-routing/README.md) · [url](https://arxiv.org/abs/2605.07111)
