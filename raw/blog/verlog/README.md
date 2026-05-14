---
title: Verlog: An Efficient Synchronized Multi-turn RL Framework for LLM Agents
url: https://openreview.net/forum?id=U3yTQonq10
type: blog
authors: [Wentse Chen, Jiayu Chen, Hao Zhu, Fahim Tajwar, Ruslan Salakhutdinov]
venue: ICLR 2026
year: 2025
topics: [agents, rl, systems]
added: 2026-05-13
---

# Verlog: An Efficient Synchronized Multi-turn RL Framework for LLM Agents

**Link:** https://openreview.net/forum?id=U3yTQonq10

## Summary
Multi-turn RL framework targeting long-horizon LLM-agent tasks with highly variable episode lengths. Combines early truncation, per-turn async rollouts, and dual-discounted GAE with pretrained value functions. First systematic 'off-policy tax' analysis. Stable beyond 400 turns on BabyAI/BabaIsAI/Crafter.

## Key points
- Per-turn async rollouts + early truncation
- Dual-discounted GAE + pretrained value functions
- Systematic off-policy tax analysis for async RL
- Stable on 400+ turn episodes
- Extends VeRL + BALROG

## See also
<!-- add [[related-slug]] links as connections form -->
