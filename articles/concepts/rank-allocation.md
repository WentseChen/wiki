# Rank Allocation

The strategy for assigning different LoRA ranks to different layers of a model. Adaptive rank allocation assigns more rank (capacity) to layers with higher gradient importance; uniform allocation gives all layers the same rank. Works well under SFT but degrades under RL fine-tuning due to flat gradient landscapes.

## Sources
- [[lora-rank-grpo]]
- [[molf-lora-full-finetuning-routing]]
