---
lng_pair: id_palimpchat
title: Complex pipelines, simple conversations
author: Gerardo Vitagliano
category: academic
tags: [academic, sigmod, llm, palimpchat]
img: "/assets/img/projects/pz_thumb.jpg"
date: 2025-06-25 16:00:00 +0200
published: true
---

<!-- outline-start -->

At SIGMOD 2025, we demonstrated PalimpChat: a conversational interface for building optimized AI data pipelines.
<!-- outline-end -->

#### Building data pipeline through natural language

Palimpzest provides a declarative way to describe AI-powered analytics, but users still need a convenient way to turn an analytical goal into a sequence of operations. [PalimpChat](https://palimpzest.org/palimpchat) explores whether that process can happen interactively through a conversation.

A user describes the task and the available data, and the system helps query the data, involving operations such as filtering, conversion, matching, or extraction. 
Different from existing systems, the conversation does not execute queries immediately but but instead generates a resulting declarative pipeline. This pipeline can be consumed by Palimpzest to optimize its execution under quality, cost, and runtime constraints.

#### Showing the system at SIGMOD

It was much fun to showcase the demo at SIGMOD 2025. Demos create a very different kind of interaction than paper talks: some of the attendees asked if they could try the system on their own data (...not on our servers unfortunately!), while others tried to stress-test it with corner cases (always have your demo on docker!).

The discussions reinforced a lesson that appears again and again in this work. Natural language can make a system easier to approach, but a useful interface still needs a solid representation and optimizer underneath it. Otherwise, the chat may sound convincing while the data pipeline remains difficult to inspect or improve.

Shout-out to Chunwei Liu, Matthew Printz, Brandon Rose, David Samson, and Mike Cafarella for the collaboration!
Find more details in the published [SIGMOD demo paper](https://dl.acm.org/doi/10.1145/3722212.3725122).

![At my poster](:palimpchat.jpg){:style="display: block; margin: auto; width: 50%;",}
