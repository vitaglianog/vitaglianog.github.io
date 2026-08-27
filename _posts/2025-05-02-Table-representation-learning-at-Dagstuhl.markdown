---
lng_pair: id_dagstuhl_table_representation
title: Dagstuhl seminar
author: Gerardo Vitagliano
category: academic
tags: [academic, dagstuhl, tables, representation learning]
img: "/assets/img/posts/dagstuhl_1.jpg"
date: 2025-05-02 12:00:00 +0200
published: true
---

<!-- outline-start -->

I spent a week at Dagstuhl discussing the challenges and opportunities of table representation learning.

<!-- outline-end -->

![Presenting my impulse talk](dagstuhl_1.jpg){:style="display: block; margin: auto; width: 50%;"}


#### My first Dagstuhl experience

Seminars in Dagstuhl have a rather unique format. The remote nature of the location and the collaborative environment create plenty of space for discussion in a relaxed yet focused environment. 
Without the usual rush between conference sessions, there is time to continue a discussion over lunch, challenge an assumption, and turn a vague idea into the beginning of a project. Some of those conversations already started shaping a potential new project around semantic data systems (...stay tuned!)

I can't not be thanful to Carsten Binnig, Madelon Hulsebos, Frank Hutter, and Julian Eisenschlos for organizing an excellent program and for having me around. The [seminar report](https://drops.dagstuhl.de/entities/document/10.4230/DagRep.15.4.126) summarizes the questions and research directions we explored.

#### Tables and beyond

Tabular data sits at an interesting intersection of community. Folks from the database, machine learning/NLP, and information retrieval communities all work with ``tables'', but each brings their unique flavors.
I would not have expected to have vivid discussion about what exactly a table is, and how to represent it! These discussions were particularly interesting to me, as they highlighted the different perspectives and assumptions that each community brings to the table (pun intended).

The Dagstuhl seminar brought these perspectives together for a week of talks, discussions, and project ideas. We discussed pretrained models for tables, multimodal data, benchmarks, data preparation, question answering, and the practical limitations that still prevent learned representations from generalizing reliably across domains.

I also gave an impulse talk titled *Beyond Tables: Multimodal Pipelines*. My main point was that a table rarely exists in isolation. Real analytical tasks connect rows with documents, images, scientific files, and other tables, so useful representations and systems must preserve both semantic meaning and structural relationships across modalities.
This insight drives my current research on declarative systems for multimodal data pipelines, and motivates my current research focus.
