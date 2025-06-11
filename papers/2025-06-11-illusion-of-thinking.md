---
title: The Illusion of Thinking Understanding the Strengths and Limitations of Reasoning Models via the Lens of Problem Complexity
date: 2025-06-11
tags:
paper: https://ml-site.cdn-apple.com/papers/the-illusion-of-thinking.pdf
code: 
year: 2025
star: 
---
Great work from Apple, it is always nice to see research that focuses on analyzing and understanding prior works, instead of pushing for marginal gains on benchmarks with the end goal of publishing. The experiments in this work compare the performance of thinking models with their non-thinking counterparts, focusing on puzzle games which have a parameter "N" that controls the problem "complexity".
- comparisons on math and puzzle environments point to a contradiction in the observed performance gaps across models and datasets, which may be attributed to data contamination during training. 
- comparisons across different "complexity" frontiers (at equal compute budgets) show that non-thinking models perform as well, or better than their reasoning counterparts at low complexity tasks.
- as complexity grows to a "critical" point, the accuracy of reasoning models drops as they fail to take advantage of additional inference compute, suggesting a fundamental scaling limitation. 
Notably, even when the solution algorithm of the puzzles is provided in the prompt, reasoning models will fail at a similar "critical" point, which underlines the title: "Illusion of Thinking".
