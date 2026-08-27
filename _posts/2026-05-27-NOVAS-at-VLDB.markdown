---
lng_pair: id_novas_vldb_2026
title: NOVAS returns at VLDB 2026
author: Gerardo Vitagliano
category: academic
tags: [academic, workshop, novas, vldb]
img: "/assets/img/thumbs/novas_thumb.jpg"
date: 2026-05-27 12:00:00 -0400
published: true
---

<!-- outline-start -->

We are organizing the second NOVAS workshop, this time at VLDB 2026 in Boston!

<!-- outline-end -->

#### NOVAS is back!

The first NOVAS workshop at SIGMOD confirmed that there is a growing community interested in the systems questions behind AI-powered data processing.
Since then, semantic operators and agentic data systems have developed quickly, making the need for shared abstractions, benchmarks, and optimization techniques even clearer.

For the second edition, we are broadening the discussion around semantic data systems.
Topics include declarative and multi-agent processing, hybrid relational-AI queries, multimodal analytics, efficient model serving, vector databases, and new architectures for relational data.

NOVAS will take place on August 31st at VLDB 2026 in Boston.
The program and all workshop information are available at [novasworkshop.org](https://www.novasworkshop.org/).

#### Our Keynotes

I am particularly excited about our [keynote lineup](https://www.novasworkshop.org/keynotes): Omar Khattab, Anupam Datta, Stratos Idreos, and Raul Castro Fernandez.
Together, their talks cover several layers of an AI system, from adapting models to a specific environment, to optimizing semantic operations, automatically designing the system itself, and building the data infrastructure needed by entire agentic organizations.

- [Omar Khattab](https://omarkhattab.com) will give a talk on *Optimizing AI Systems at the Last Mile*.
As foundation models become more capable, broad and one-size-fits-all competence gets cheaper, but adapting a system to the specific information and constraints of a downstream environment remains difficult.
The talk will connect recent work on Recursive Language Models, Machine Studying, and Pedagogical RL to explore how systems can process long prompts, study large collections of information, and learn more efficiently from qualitative feedback.
- [Anupam Datta](https://www.snowflake.com/en/blog/authors/anupam-datta/) will present *Cortex AI SQL*, Snowflake's production SQL engine for combining relational queries with native semantic operations over structured and unstructured data.
Traditional optimizers are not designed for operations whose cost, latency, and selectivity depend on model inference.
The talk will describe how Cortex AI SQL treats inference cost as part of query optimization, uses adaptive model cascades to balance quality and efficiency, and rewrites expensive semantic joins into more scalable operations.
I am particularly curious to hear the lessons learned from deploying these techniques on real Snowflake customer workloads.

- [Stratos Idreos](hhttps://stratos.idreos.ai/) will discuss *Self-designing AI*.
His starting point is that powerful models and agent frameworks are components, but not complete systems: organizations still need to assemble, evaluate, and continuously adapt many specialized models and agents.
The talk proposes an infrastructure where a small set of computational primitives can be composed through automated search to create systems tailored to their workload and constraints.
One example is LegoAI, which automatically designs language-model training algorithms and was productized as TorchTitan in PyTorch.

- [Raul Castro Fernandez](https://www.raulcastrofernandez.com) will talk about *Building the Data Infrastructure for Agentic Organizations*.
As agents become active participants in organizations, dataflows determine what information they can access, how efficiently they can act, and how their behavior can be governed.
The talk will introduce a data ecology perspective through systems such as Pneuma for structured data work, internal data markets for allocating valuable context, and existential documents for governing organizational dataflows.

I like how these four talks approach the same broad question from different directions: how can we turn increasingly powerful AI components into systems that are efficient, adaptable, and useful in the real world?

#### From Vibe Researcher to Vibe Entrepreneur

This year, we are also hosting a panel titled [*From Vibe Researcher to Vibe Entrepreneur*](https://www.novasworkshop.org/panel).
The question we are asking is: what does it take to turn a promising academic semantic data system into a useful product?
The panel brings together five perspectives on that transition:

- Çağla Kaymaz, Partner at Category VC, who invests in AI and data infrastructure companies and works with many teams founded by PhDs.
- Tim Kraska, Professor at MIT and co-founder of Instancio and Einblick Analytics, both of which were acquired.
- Ajay Rayasam, Principal at OUP VC, with experience in technology investing, startup product management, and fundraising.
- Fatma Ozcan, Principal Engineer at Google Systems Research, with more than two decades of experience turning data management research into industrial technology.
- Rana Shahout, Postdoctoral Fellow at Harvard, whose research focuses on efficient and scalable AI systems and LLM inference.

The panel will take place at 4:20 PM in Grand Ballroom E.

Many thanks to Paolo Papotti, Chunwei Liu, Liana Patel, Rana Shahout, and Andreas Kipf for organizing this edition with me, and to everyone contributing papers, reviews, and ideas.
I am looking forward to another day full of ambitious ideas and practical systems questions :)
