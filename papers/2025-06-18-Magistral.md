---
title: Magistral
date: 2025-06-18
tags:
paper: https://arxiv.org/pdf/2506.10910
code: https://huggingface.co/mistralai/Magistral-Small-2506
year: 2025
star: true
---
Technical report from Mistral, lots of details + experiments on training reasoning models at scale. Interesting findings for me were:
- They reinforce the changes to GRPO proposed by others (Dr.GRPO, DAPO, Clip Higher, etc.). Remove KL divergence, token-level loss to avoid length bias, normalize the advantage on the batch level (not group), raise the clipping threshold (for high), dynamic sampling (to eliminate non diverse groups).
- Another example showing SFT Cold start + RL is better than RL or SFT alone (Table 3).
- Figure 8 gives some intuition about how RL improves performance: as parameters evolve during training, prompt length and mean reward grow in unison. This follows a log-scaling relationship, supporting the claim that inference time compute is key to scaling RL.