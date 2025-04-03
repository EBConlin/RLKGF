# RLKGF
Reinforcement learning knowledge graph feedback for LLM tuning.

TLDR - Build algorithm for quickly checking node reachability and estimate a path. Combines embedding and summarization tactics. But, unlike HARP or GraphZoom, doesn't disgard lower-level embedding spaces.
In order too...
Instead of using a neural net to infer human feedback (RLHF), build a knowledge graph sufficient to provide human feedback on a particular subject and a means for query optimization.


My goal has been to experiment with LLM assistants useful to scientists given the rise in scientific databases where entriers include both data and paper(eg recent NIH NWB initiative for neuroscience). We need..
I wanted to use LLMs interfaces between scientists and massive databases of past findings/data. I broke the problem down into...
1. A means of parsing research publications argumentative structure -> Knowledge Graph. Eventually I'd want to include data sources as nodes which are sampled from a hidden dimension.
2. Tuning the LLM would be helped by building ways to quickly check if two nodes (scientific premises) are connected (logically infer one another) or don't (irrelevant or proximal and contradictory), and ways to quickly estimate a "good enough" path.

This repo is an implementation of 2 without 1 (which is being improved) on a citation network
