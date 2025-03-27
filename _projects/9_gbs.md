---
title: "Lexically Constrained Decoding of Transformers"
duration: "2025.02-2025.03"
excerpt: "In a class project, we adapt the constrained decoding algorithm Grid Beam Search (GBS) to impose lexical constraints on transformers. GBS was originally applied to stateful Neural Translation Models for seq2seq translation tasks. We develop a new pipeline for generating structured outputs from a given prompt and set of lexical constraints that supports any pretrained autoregressive language model, which we choose to be GPT2. Then, we fine-tune GPT-2 on a corpus of Chekhov's stories. Our subjective analysis also showed that GBS + fine-tuned GPT2 gave more interesting and meaningful domain-specific results than GBS + GPT2 alone."
collection: projects
paper: /files/gbs_paper.pdf
code: https://github.com/ilanashapiro/constrained_decoding_gbs_transformers
slides: https://docs.google.com/presentation/d/1XNCqX4Eab9vS3RscQFMXXLrzUaGAJc-_I9JRulo6qjc/edit?usp=sharing
image: gbs.png
---