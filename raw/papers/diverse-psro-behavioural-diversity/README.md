---
title: Modelling Behavioural Diversity for Learning in Open-Ended Games
url: https://arxiv.org/abs/2103.07927
type: paper
authors: [Nicolas Perez-Nieves, Yaodong Yang, Oliver Slumbers, David H Mguni, Ying Wen, Jun Wang]
venue: ICML
year: 2021
topics: [rl, game-theory, agents]
added: 2026-05-11
arxiv_id: 2103.07927
---

# Modelling Behavioural Diversity for Learning in Open-Ended Games

**Link:** https://arxiv.org/abs/2103.07927

## Summary
Gives a geometric definition of behavioural diversity in normal-form and open-ended games and operationalizes it as a determinantal-point-process (DPP) kernel over policies. Plugs the DPP-diversity term into best-response training, yielding Diverse Fictitious Play and Diverse PSRO that find lower-exploitability, more behaviorally varied populations than vanilla PSRO.

## Key points
- Formal geometric definition of behavioural diversity in games.
- DPP-based diversity metric over policy payoff features.
- Diverse PSRO: diversity-regularized best-response oracle.
- Lower exploitability than PSRO across many normal-form / open-ended games.
- Complements [[open-ended-learning-symmetric-zero-sum]] (Rectified Nash).

## See also
- [[open-ended-learning-symmetric-zero-sum]]
- [[unified-game-theoretic-marl]]
