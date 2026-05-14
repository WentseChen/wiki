---
title: "Parameter Efficient Reinforcement Learning from Human Feedback"
url: https://arxiv.org/abs/2403.10704
type: paper
authors: [Hakim Sidahmed, Samrat Phatale, Alex Hutcheson, Zhuonan Lin, Zhang Chen, Zac Yu, Jarvis Jin, Simral Chaudhary, Roman Komarytsia, Christiane Ahlheim, Yonghao Zhu, Bowen Li, Saravanan Ganesh, Bill Byrne, Jessica Hoffmann, Hassan Mansoor, Wei Li, Abhinav Rastogi, Lucas Dixon]
year: 2024
topics: [rl, nlp]
added: 2026-05-14
arxiv_id: "2403.10704"
---

# Parameter Efficient Reinforcement Learning from Human Feedback

**Link:** https://arxiv.org/abs/2403.10704

## Summary

This paper provides a large-scale empirical evaluation of parameter-efficient RLHF (PE-RLHF) using LoRA for both reward modeling and policy optimization. Benchmarked across six datasets covering summarization, response generation, UI automation, and visual question answering, PE-RLHF achieves comparable performance to full RLHF while providing substantial efficiency gains: up to 90% faster reward model training, 30% faster RL training, 50% memory reduction for reward models, and 27% memory reduction for RL.

The study's breadth — six tasks, multiple model sizes, both reward modeling and policy fine-tuning phases — makes it a key reference for understanding where LoRA can and cannot substitute for full fine-tuning in the RLHF pipeline. The comparable performance finding is particularly notable given that LoRA tunes only a small fraction of parameters.

## Key points

- PE-RLHF matches full RLHF performance across 6 diverse datasets (summarization, VQA, UI automation, etc.).
- 90% faster reward model training and 50% memory reduction vs. full RLHF.
- 30% faster RL policy training and 27% memory reduction vs. full RLHF.
- Evaluates LoRA for both reward model fine-tuning and policy optimization phases.
- Large-scale empirical study establishing PE-RLHF as a practical drop-in for full RLHF.

## See also
<!-- [[lora-rlhf-efficiency-regularization]] [[lora-rank-grpo]] -->
