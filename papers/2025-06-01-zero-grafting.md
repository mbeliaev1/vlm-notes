---
title: Zero-Shot Vision Encoder Grafting via LLM Surrogates
date: 2025-06-01
tags:
paper: https://arxiv.org/abs/2505.22664
code: https://github.com/facebookresearch/zero
year: 2025
star: 
---
Introduce zero-shot grafting: train a vision encoder on a smaller surrogate LM that shares the same embedding space as the large LM, then *graft* the encoder to the large LM. Show that training costs decrease up to 45% while achieving comparable accuracy as end-to-end training. 
