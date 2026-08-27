---
lng_pair: id_kramabench
title: KramaBench and real-world data science pipelines
author: Gerardo Vitagliano
category: academic
tags: [academic, benchmark, ai, data science]
img: "/assets/img/thumbs/kramabench_thumb.png"
date: 2026-05-01 18:00:00 -0400
meta_modify_date: 2026-04-24 18:00:00 -0300
published: true
---

<!-- outline-start -->
![A sample task in KramaBench](:kramabench_task.png){:style="display: block; margin: auto; width: 100%;"}

KramaBench is a benchmark whether AI systems can design and execute complete data-to-insight pipelines over real data lakes.

<!-- outline-end -->

#### From isolated questions to complete pipelines

AI systems are increasingly expected to behave like data scientists. A realistic task may require finding the relevant files, understanding their schemas, cleaning and integrating them, choosing a statistical method, and finally producing an answer. Evaluating only one isolated step misses much of what makes these workflows difficult.

[KramaBench](https://kramabench.org/) contains 104 manually curated tasks over 1,700 real files from six domains: archaeology, astronomy, biomedical research, environmental science, legal discovery, and wildfire prevention. The tasks evaluate both pipeline design and implementation, which lets us distinguish between a system that has a plausible plan and one that can actually execute it correctly.

The name is a reference to *Vinyasa Krama*. In Sanskrit, *krama* means sequence or order, which fits a benchmark where the transitions between steps matter just as much as the individual operations.

#### From the benchmark to ICLR

This was a huge collaborative effort involving researchers across MIT, who contributed to manually designing and verifying all tasks and reference solutions. 
The results show that current systems can make meaningful progress, but complete real-world pipelines remain difficult. In particular, correctly implementing a pipeline is often much harder than describing a reasonable design for it.

![Presenting KramaBench at ICLR](:iclr_2.png){:style="display: block; margin: auto; width: 100%;"}

I am very happy that the work was accepted at ICLR 2026, where I have presented it in Rio! It was great to discuss the benchmark with the research community and hear how others are thinking about autonomous data science agents.

The [paper](https://proceedings.iclr.cc/paper_files/paper/2026/file/e7132f7446c0d61726c523a1af7a6a74-Paper-Conference.pdf), [code](https://github.com/mitdbg/kramabench), data, and leaderboard are all available online.
If you are developing the new generation of AI data science agents, we hope you will try your system on KramaBench and share your results!
