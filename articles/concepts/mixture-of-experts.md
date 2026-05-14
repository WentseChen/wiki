# Mixture of Experts (MoE)

Architecture where a router selects a sparse subset of specialized sub-networks (experts) to process each input. In LoRA contexts, MoE routing over singular value priors from pretrained weights enables adaptive low-rank subspace selection, recovering capacity lost by static rank assignment.

## Sources
- [[goat-lora-adaptive-svd-moe]]
- [[remix-rl-routing-mixture-loras]]
