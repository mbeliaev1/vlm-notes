---
title: Can Reasoning Scale?         
date:  2025-06-11                
tags:    
links:                         
---
The "million dollar question", though today that number feels orders of magnitude larger. I am sure that most people who have worked with RL in the past are wondering the same thing. The flood of tech media, supported by research from both frontier labs and academia, will have you bet the house. The risk-reward tradeoff looks too good to pass up.

That is why it is refreshing to see research that goes against the grain, focusing on analyzing prior works, instead of pushing for marginal gains on benchmarks with the end goal of publishing. Yes, I am referring to the recent "Illusion of Thinking" paper from *Apple* (which I summarized here: [2025-06-11-illusion-of-thinking](../papers/2025-06-11-illusion-of-thinking.md)). Taken at face value, we start to question the prevailing training recipe: autoregressive language modeling -> SFT on instruction based prompts-> multi-phase RL. Can sparse, verifiable reward signals truly guide pretrained language models to develop generalizable *thinking* abilities?

To me, the core challenge in teaching models to reason with RL is this: **how do we define a signal that reflect actual “understanding” of data beyond memorization?** Reinforcing an educated guess through RL may not be enough. As *preconditioned* humans, we seem to possess an intuitive grasp of *how to reason*. When reading a paper, confusion may sometimes spark a new chain of thought. At other times, we may deliberately defer understanding, anticipating that future information will make things clear. 

But should we try to hard-code human biases into the training process? Or is it better to let the model discover its own method for reasoning, embracing the "bitter lesson" that hand-designed heuristics fall short in the long run? 