# Wiki index

Master entry point. Browse by topic, or scan recent additions below.

## Topics

- [nlp](topics/nlp.md) — language models, training, alignment, prompting, evaluation
- [rl](topics/rl.md) — reinforcement learning
- [agents](topics/agents.md) — agentic systems, tool use, multi-agent
- [self-play](topics/self-play.md) — self-play training
- [game-theory](topics/game-theory.md) — game theory
- [multimodal](topics/multimodal.md) — VLMs, multimodal
- [vision](topics/vision.md) — computer vision
- [systems](topics/systems.md) — ML systems, infra
- [continuous-learning](topics/continuous-learning.md) — continual learning
- [theory](topics/theory.md) — learning theory
- [bandit](topics/bandit.md) — bandits
- [ml](topics/ml.md) — general ML
- [others](topics/others.md) — misc

## Recent additions

- [[primacy-bias-deep-rl]] — Periodic resets of the last few layers cure deep RL's overfitting to early data and unlock high replay ratios. *Nikishin et al., 2022.*
- [[dormant-neuron-phenomenon]] — Hidden units go "dormant" during DQN training; ReDo periodically reinitializes them to restore capacity. *Sokar et al., 2023.*
- [[capacity-loss-rl]] — Non-stationary TD targets shrink feature rank; InFeR regularizes features toward init to preserve capacity. *Lyle et al., 2022.*
- [[implicit-under-parameterization]] — Bootstrapped value learning collapses the feature matrix to low effective rank in deep RL. *Kumar et al., 2021.*
- [[warm-starting-shrink-perturb]] — Continued training generalizes worse than from-scratch; shrink-and-perturb closes the gap. *Ash & Adams, 2020.*
- [[l2-init-regenerative]] — L2-regularize toward initial parameters (not zero) to preserve plasticity in continual supervised learning. *Kumar et al., 2023.*
- [[plasticity-loss-continual-drl]] — Plasticity loss clearly demonstrated on continual Atari; CReLU activations largely mitigate it. *Abbas et al., 2023.*
- [[understanding-plasticity-nn]] — Plasticity loss is driven by loss-landscape curvature blowup; dead units are downstream symptoms. *Lyle et al., 2023.*
- [[ewc-elastic-weight-consolidation]] — Quadratic penalty around each task's weights (Fisher-weighted) overcomes catastrophic forgetting. *Kirkpatrick et al., 2017.*
- [[plasticity-injection-drl]] — Zero-impact residual injection adds trainable capacity and serves as a causal plasticity diagnostic. *Nikishin et al., 2023.*
- [[plasticity]] — Deep nets lose plasticity under continual training; continual backprop (reinit least-used units) restores it. *Dohare et al., 2024.*
- [[diayn-skill-discovery]] — Unsupervised skill discovery via MI between latent skill and visited states. *Eysenbach et al., 2019.*
- [[dvd-population-diversity]] — Population diversity as determinant of kernel over behavioral embeddings. *Parker-Holder et al., 2020.*
- [[smerl-structured-maxent-rl]] — Multiple near-optimal solutions in one MDP via latent-gated diversity bonus. *Kumar et al., 2020.*
- [[diverse-successor-features]] — CMDP framing of diverse-near-optimal RL with SF-correlation diversity. *Zahavy et al., 2021.*
- [[domino-diversity-near-optimality]] — CMDP framing of diverse RL using state-occupancy distance. *Zahavy et al., 2022.*
- [[novelty-search-abandoning-objectives]] — Pure-novelty search beats objective-based search on deceptive tasks. *Lehman & Stanley, 2011.*
- [[map-elites]] — QD algorithm filling a discretized behavior-space archive with elites. *Mouret & Clune, 2015.*
- [[dads-dynamics-aware-skills]] — Unsupervised skills that are both diverse and predictable, enabling latent-space MPC. *Sharma et al., 2020.*
- [[icm-curiosity-driven-exploration]] — Curiosity = forward-model error in inverse-model feature space. *Pathak et al., 2017.*

<!-- newest at top, cap 20 — managed by /wiki-ingest -->
