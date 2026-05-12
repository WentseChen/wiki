---
title: Discovering Diverse Nearly Optimal Policies with Successor Features
url: https://arxiv.org/abs/2106.00669
type: paper
authors: [Tom Zahavy, Brendan O'Donoghue, Andre Barreto, Volodymyr Mnih, Sebastian Flennerhag, Satinder Singh]
venue: ICML LifelongRL workshop
year: 2021
topics: [rl]
added: 2026-05-12
arxiv_id: 2106.00669
---

# Discovering Diverse Nearly Optimal Policies with Successor Features

**Link:** https://arxiv.org/abs/2106.00669

## Summary

Frames diverse policy discovery as a CMDP: maximize a diversity reward subject to a near-optimality constraint on the task reward. The diversity reward minimizes correlation between successor features across the policy set, which the paper argues is more stable than discrimination-based diversity objectives that can collapse to suboptimal solutions.

## Key points
- CMDP formulation: diversity is the objective, task performance is a constraint.
- Successor-feature correlation is the inter-policy distance metric.
- Identifies failure modes of discrimination-based diversity (e.g. DIAYN-style) when forced near-optimality.
- Demonstrated on DeepMind Control Suite with qualitatively different locomotion gaits.

## See also
- [[reward-switching-policy-optimization]]
- [[smerl-structured-maxent-rl]]
- [[domino-diversity-near-optimality]]
