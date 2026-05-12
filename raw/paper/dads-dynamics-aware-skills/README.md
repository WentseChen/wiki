---
title: Dynamics-Aware Unsupervised Discovery of Skills
url: https://arxiv.org/abs/1907.01657
type: paper
authors: [Archit Sharma, Shixiang Gu, Sergey Levine, Vikash Kumar, Karol Hausman]
venue: ICLR
year: 2020
topics: [rl]
added: 2026-05-12
arxiv_id: 1907.01657
---

# Dynamics-Aware Unsupervised Discovery of Skills (DADS)

**Link:** https://arxiv.org/abs/1907.01657

## Summary

DADS learns a continuous latent skill space jointly with skill-conditioned dynamics models, where each skill is encouraged to be both diverse and predictable in its effect on the environment. Because skills are predictable, downstream tasks can be solved by model-predictive control in the latent skill space rather than the raw action space, giving strong zero-shot planning and sparse-reward performance.

## Key points
- Mutual-information objective like DIAYN, but conditioned to make skills predictable.
- Joint learning of skill policy and skill-conditioned dynamics model.
- Plans in latent skill space → zero-shot transfer on downstream tasks.
- Continuous skill latent → effectively infinite skill repertoire.

## See also
- [[diayn-skill-discovery]]
- [[reward-switching-policy-optimization]]
