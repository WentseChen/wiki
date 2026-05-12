---
title: "α-Rank: Multi-Agent Evaluation by Evolution"
url: https://arxiv.org/abs/1903.01373
type: paper
authors: [Shayegan Omidshafiei, Christos Papadimitriou, Georgios Piliouras, Karl Tuyls, Mark Rowland, Jean-Baptiste Lespiau, Wojciech Czarnecki, Marc Lanctot, Julien Perolat, Remi Munos]
venue: Nature Scientific Reports
year: 2019
topics: [rl, game-theory, agents]
added: 2026-05-11
arxiv_id: 1903.01373
---

# α-Rank: Multi-Agent Evaluation by Evolution

**Link:** https://arxiv.org/abs/1903.01373

## Summary
Proposes α-Rank, an evolutionary-dynamics ranking method for multi-agent systems based on Markov-Conley chains. Unlike Nash, it is unique, polynomial-time computable, and applies to general-sum, many-player, symmetric or asymmetric empirical games — making it a practical drop-in meta-solver for PSRO-style population learning. Validated on AlphaGo, AlphaZero, MuJoCo Soccer, and Poker.

## Key points
- Ranking grounded in Markov-Conley chains, a new dynamical solution concept.
- Polynomial-time in the number of pure strategies (Nash is intractable in general).
- Scales to symmetric/asymmetric games and arbitrary player counts.
- Provides strengths/weaknesses and long-run dynamics, not just a scalar score.
- Foundation for α-PSRO (see [[alpha-psro-generalized-training]]).

## See also
- [[unified-game-theoretic-marl]]
- [[alpha-psro-generalized-training]]
