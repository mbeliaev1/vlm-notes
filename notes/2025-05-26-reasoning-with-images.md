---
title: Reasoning with Images         
date:  2025-05-26                
tags:    
links:                         
---
Just finished the backlog of preprints I received from arxiv, amplified by the recent NeurIPS deadline receiving 25 THOUSAND submissions! One topic stood out in a few of the papers: Using RL to improve the reasoning capabilities of VLMs ([2025-05-26-pixel-reasoner](./papers/2025-05-26-pixel-reasoner.md),[2025-05-26-visionary-r1](papers/2025-05-26-visionary-r1.md),[2025-05-26-grit](papers/2025-05-26-grit.md),[2025-05-26-vlm-r3](papers/2025-05-26-vlm-r3.md),[2025-05-26-vision-reasoner](papers/2025-05-26-vision-reasoner.md),[2025-05-26-observe-r1](papers/2025-05-26-observe-r1.md),[2025-05-26-g1](papers/2025-05-26-g1.md),[2025-05-26-difficulty-prior](papers/2025-05-26-difficulty-prior.md),[2025-05-26-deepeyes](papers/2025-05-26-deepeyes.md),[2025-05-26-r1-sharevl](papers/2025-05-26-r1-sharevl.md).) The subset of papers listed shared a few key insights: 
- Vision needs to be grounded in the reasoning output. These methods often introduce specific tags (perception, bounding box, caption, etc.) that force the model to interleave images with text, and provide verifiable reward signals that provide feedback to the content within these tags.  
- RL can be used to train small VLMs without SFT cold start. While this point was often underlined by the authors, it is unclear if this observation stems from access to multi-part reward signals (caption/bounding box/correctness) in the data available. 
- Learning needs to be difficulty aware, especially when using GRPO as "too easy" and "too hard" prompts leads to bad advantage estimation in response groups. Additional heuristic signals are often provided to facilitate dynamic sampling.  