---
title: Illuminating Search Spaces by Mapping Elites
url: https://arxiv.org/abs/1504.04909
type: paper
authors: [Jean-Baptiste Mouret, Jeff Clune]
venue: arXiv
year: 2015
topics: [rl]
added: 2026-05-12
arxiv_id: 1504.04909
---

# MAP-Elites: Illuminating Search Spaces by Mapping Elites

**Link:** https://arxiv.org/abs/1504.04909

## Summary

MAP-Elites is the foundational quality-diversity algorithm: it discretizes a user-defined behavior space into cells and keeps the highest-performing solution in each cell, producing an archive that "illuminates" how performance varies across behavior dimensions. The archive itself is the output — a population of qualitatively distinct high-performing solutions rather than a single optimum.

## Key points
- Behavior space is discretized into cells; each cell holds one elite.
- Produces a diverse high-performing archive, not a single best solution.
- Validated on modular neural nets, soft robots, and physical robot design.
- Backbone of modern QD literature; conceptual ancestor of RSPO-style iterative diverse-policy discovery.

## See also
- [[novelty-search-abandoning-objectives]]
- [[reward-switching-policy-optimization]]
