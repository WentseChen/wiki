---
title: Deep Reinforcement Learning from Self-Play in Imperfect-Information Games
url: https://arxiv.org/abs/1603.01121
type: paper
authors: [Johannes Heinrich, David Silver]
venue: arXiv
year: 2016
topics: [rl, game-theory, self-play]
added: 2026-05-11
arxiv_id: 1603.01121
---

# Deep Reinforcement Learning from Self-Play in Imperfect-Information Games

**Link:** https://arxiv.org/abs/1603.01121

## Summary
Introduces Neural Fictitious Self-Play (NFSP) — the first scalable end-to-end approach to approximating Nash in imperfect-information games without domain knowledge or handcrafted abstractions. Combines fictitious self-play with deep RL: a Q-network learns best responses, a policy network learns the average strategy via supervised learning. Converges to Nash in Leduc poker where independent RL diverges, and matches state-of-the-art expert-engineered programs in limit Texas Hold'em. Predecessor and baseline for PSRO.

## Key points
- First end-to-end deep-RL Nash solver for imperfect-info games.
- Two networks: best-response (Q-learning) + average-strategy (supervised).
- Converges to Nash on Leduc; independent Q-learning does not.
- Competitive with handcrafted superhuman limit Texas Hold'em programs.
- Direct predecessor of PSRO; standard baseline in subsequent work.

## See also
- [[unified-game-theoretic-marl]]
- [[escher-eschewing-importance-sampling]]
