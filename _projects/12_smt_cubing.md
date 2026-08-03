---
title: "Parallelizing SMT Solvers via Dynamic Partitioning, Core-Guided Search-Space Pruning, and Online Backbone Detection"
duration: "2025.07-2026.05"
excerpt: "At Microsoft Research, I worked with [Nikolaj Bjørner](https://www.microsoft.com/en-us/research/people/nbjorner/) to design and implement a novel parallel framework for the [Z3](https://www.microsoft.com/en-us/research/project/z3-3/) SMT solver that uses *feedback from active search* to steer solving. Our approach dynamically builds a *binary partition tree* of the search space by sampling from workers' VSIDS statistics during solving. We introduced a novel search-space pruning mechanism that harnesses the full power of *core-based CDCL-style pruning* to continuously shrink the partition tree. We further optimized our architecture by incorporating *online backbone detection* into worker threads, as well as a *terminate-on-demand* mechanism to eagerly eliminate work on pruned subproblems. The resulting algorithm is highly generalizable and scalable. The implementation can be found [here](https://github.com/Z3Prover/z3/blob/master/src/smt/smt_parallel.cpp) and was released in [z3-5.0.0](https://github.com/Z3Prover/z3/releases/tag/z3-5.0.0)."
collection: projects
selected: true
image: parallel_z3.png
paper: https://arxiv.org/abs/2606.08852
code: https://github.com/Z3Prover/z3/blob/master/src/smt/smt_parallel.cpp
slides: https://docs.google.com/presentation/d/1Uun3pFt0PpUNnBI8jjnfFnyF_RAoo_uFHG9wwSBHFP0/edit?usp=sharing
report: /files/smtcomp2026_z3.pdf
---
