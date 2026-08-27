---
lng_pair: id_palimpzest
title: Optimizing AI workloads with Palimpzest
author: Gerardo Vitagliano
category: academic
tags: [academic, data systems, llm, palimpzest]
img: "/assets/img/projects/pz_thumb.jpg"
date: 2024-05-24 10:00:00 -0400
published: true
---

<!-- outline-start -->

Introducing Palimpzest, a declarative system for building and optimizing AI-powered data pipelines.

<!-- outline-end -->

#### Dreadful AI Pipelines

Modern data pipelines increasingly mix traditional transformations with expensive AI operations: extracting information from documents, interpreting images, matching entities, or answering semantic questions. Building such a pipeline is already complicated. Choosing which model to use for every operation, and deciding how to trade quality for time and cost, makes it even harder.

The usual approach is to encode all of these decisions directly into executable scripts. But if you do that, you are essentially hardcoding the decisions into the code, which makes it difficult to adapt to new situations or improve the pipeline over time. A new model is out? You want to try a better execution strategy presented last week at NeurIPS? Tough luck, you should rewrite all your pipelines yourself.
Does this problem sound familiar to you?

#### Declarative optimization to the rescue!

[Palimpzest](https://www.palimpzest.org/) separates what the user wants to compute from how the system executes it. 
In true declarative spirit, like SQL, users describe the logical operations and the desired quality, cost, or runtime constraints. The system can then search over alternative physical plans involving different models, prompts, and execution strategies.

This is a familiar idea in database systems: SQL users state the result they want, while a query optimizer decides how to produce it. Palimpzest explores what that idea looks like for AI-powered analytics, where operations are probabilistic and the cheapest plan may not be the most accurate one.

This has been a very exciting project to work on at CSAIL. The system is open source on [GitHub](https://github.com/mitdbg/palimpzest), and our paper [Palimpzest: Optimizing AI-Powered Analytics with Declarative Query Processing](https://arxiv.org/abs/2405.14696), describes the ideas in more detail.
