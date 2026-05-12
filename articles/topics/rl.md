# rl

Reinforcement learning — policy/value methods, exploration, offline RL.

## Overview

<!-- short overview, maintained by LLM as the topic grows -->

## Key concepts

<!-- bullet list of [[concept-slug]] links into articles/concepts/ -->

## Recent

- [[reward-switching-policy-optimization]] — Iteratively discovers diverse policies by switching extrinsic/intrinsic reward on trajectory novelty. *Zhou et al., 2022.*
- [[neupl-neural-population-learning]] — One conditional net represents the whole PSRO population, all policies trained concurrently. *Liu et al., 2022.*
- [[anytime-psro]] — APSRO picks a meta-distribution that monotonically decreases exploitability vs the full game. *McAleer et al., 2022.*
- [[jpsro-correlated-equilibrium]] — JPSRO uses (C)CE meta-solvers + MGCE selection; extends PSRO to n-player general-sum games. *Marris et al., 2021.*
- [[diverse-psro-behavioural-diversity]] — Diverse PSRO with a DPP diversity kernel; lower exploitability on open-ended games. *Perez-Nieves et al., 2021.*
- [[xdo-extensive-form-double-oracle]] — Mixes best responses at every infostate; linear-in-infostates Nash convergence. *McAleer et al., 2021.*
- [[pipeline-psro]] — Parallel PSRO via hierarchical RL workers; SOTA on Barrage Stratego with guarantees preserved. *McAleer et al., 2020.*
- [[alpha-psro-generalized-training]] — α-PSRO: uses α-Rank as meta-solver, extending PSRO to general-sum many-player games. *Muller et al., 2020.*
- [[alpha-rank]] — Markov-Conley-chain ranking; unique, polynomial-time, drop-in PSRO meta-solver. *Omidshafiei et al., 2019.*
- [[open-ended-learning-symmetric-zero-sum]] — Rectified Nash Response: niching best-response for nontransitive games. *Balduzzi et al., 2019.*
- [[neural-fictitious-self-play]] — NFSP: deep-RL fictitious play, first scalable Nash solver for imperfect-info games. *Heinrich & Silver, 2016.*
- [[unified-game-theoretic-marl]] — PSRO: best-response RL against an empirical-game meta-strategy; diagnoses multiagent overfitting via joint-policy correlation. *Lanctot et al., 2017.*

<!-- newest at top — managed by /wiki-ingest -->
