# The Primacy Bias in Deep Reinforcement Learning

*paper, 2022. Nikishin, Schwarzer, D'Oro, Bacon, Courville.*

Identifies a "primacy bias" in deep RL: high-update-ratio agents irreversibly overfit to their earliest few thousand transitions. A simple periodic reset of the last few layers (keeping the replay buffer) unlocks much higher replay ratios and lifts SAC/DrQ/SPR on Atari-100k and DMC.

→ [raw entry](../../raw/paper/primacy-bias-deep-rl/README.md) · [url](https://arxiv.org/abs/2205.07802)
