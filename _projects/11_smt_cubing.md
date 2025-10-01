---
title: "Parallelizing Z3: Adaptive Cubing via On-The-Fly Sampling of CDCL Conflict Traces"
duration: "2025.07-2025.9"
excerpt: "At Microsoft Research, I worked with [Nikolaj Bjorner](https://www.microsoft.com/en-us/research/people/nbjorner/) to design and implement a novel parallelization algorithm for the SMT solver Z3. We developed an online cube-and-conquer approach, where cubes are dynamically sampled during solving from CDCL conflict-variable heuristics. Cubes are distributed to worker threads based on similarity, allowing each thread to maximize reuse of its existing solver state. My contribution was merged into Z3's master branch. See [my fork](https://github.com/ilanashapiro/z3/blob/parallel-solving/src/smt/smt_parallel.cpp) for the experimental versions at the end of my internship, or the [main repo](https://github.com/Z3Prover/z3/blob/master/src/smt/smt_parallel.cpp) for the merged code. Currently, we are exploring adding online parameter tuning."
collection: projects
image: parallel_cubing.png
slides: https://docs.google.com/presentation/d/1fG-2aDKSI7zXmeVLD6aNk_5dQ2f9KXjodczDli39O_Q/edit?usp=sharing
---