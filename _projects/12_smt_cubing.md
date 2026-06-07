---
title: "Parallelizing SMT Solvers via Dynamic Partitioning, Core-Guided Search-Space Pruning, and Online Backbone Detection"
duration: "2025.07-2026.05"
excerpt: "At Microsoft Research, I worked with [Nikolaj Bjørner](https://www.microsoft.com/en-us/research/people/nbjorner/) to design and implement a novel parallel framework for SMT solvers that dynamically builds a binary partition tree of the search space by sampling from worker threads’ VSIDS statistics during solving. We leverage the full power of core-based CDCL-style pruning to continuously shrink the partition tree. We further optimize our architecture by incorporating online backbone detection into worker threads, as well as a terminate-on-demand mechanism to eagerly eliminate work on pruned subproblems. The resulting algorithm is highly generalizable and scales effectively with available resources. The implementation can be found [here](https://github.com/Z3Prover/z3/blob/master/src/smt/smt_parallel.cpp)."
collection: projects
image: parallel_z3.png
slides: https://docs.google.com/presentation/d/1Uun3pFt0PpUNnBI8jjnfFnyF_RAoo_uFHG9wwSBHFP0/edit?usp=sharing
---