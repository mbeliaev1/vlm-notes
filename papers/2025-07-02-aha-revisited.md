---
title: Aha Moment Revisited Are VLMs Truly Capable of Self Verification in Inference-time Scaling?
date: 2025-07-02
tags:
paper: https://arxiv.org/pdf/2506.17417
code: 
year: 2025
star: 
---
Provide empirical evidence that inference time "aha-moments" learned via RL do not translate into practical self-verification gains for VLMs. Generation strategies such as majority vote still outperform verification strategies, revealing a gap that is potentially rooted in weak visual self-checking. Interestingly, when images are removed from the verification input, performance improves, suggesting that purely using outcome rewards for fine tuning is not enough too illicit multi-modal reasoning. This observation is supported by other research which emphasizes grounding visual reasoning when training: [2025-05-26-g1](../papers/2025-05-26-g1.md).
