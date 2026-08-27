---
lng_pair: id_autosynthesis
title: AutoSynthesis and automated meta-analysis
author: Gerardo Vitagliano
category: academic
tags: [academic, agents, meta-analysis, llm]
img: "/assets/img/posts/autosynthesis.png"
date: 2026-07-16 14:00:00 -0400
published: true
---

<!-- outline-start -->

AutoSynthesis is an agentic system that automates the steps of a scientific meta-analysis while keeping the process transparent.

<!-- outline-end -->

#### Automating meta-analysis

The goal of meta-analysis is to turn results from many individual studies into a quantitative summary of the available evidence. 
It is an essential tool in scientific domains like social science and medicine, but the workflow remains remarkably manual. Researchers must formulate a search, screen papers, assess eligibility, extract statistics, reconcile different measurements, and finally run the statistical analysis.

This project was born as a collaboration with Moein Taherinezhad, Sebastian Maier, Francesco Pierri, and Stefan Feuerriegel. We asked ourselves: could we automate this workflow using a combination of specialized agents, while keeping the process transparent enough to be auditable by human researchers?

[AutoSynthesis](https://arxiv.org/abs/2607.15247) is a framework of specialized agents designed to tackle the complete meta-analysis workflow. Starting from a research question, the system retrieves literature, screens candidate studies, extracts quantitative claims, computes standardized effect sizes, performs a random-effects meta-analysis, and produces a report aligned with PRISMA guidelines.

#### Interdisciplinary challenges

The interesting systems challenge is not merely connecting several model calls. Evidence synthesis requires intermediate decisions to remain inspectable: why a study was included, where a statistic came from, how an effect size was computed, and which assumptions entered the final estimate.

In our first experiments, we tested AutoSynthesis on 28 studies and extracted over 20 quantitative claims. Its pooled estimates were close to those from expert-conducted analyses. 
This encouraging results are a stepping stone towards reducing the burden on researchers and accelerating the time required for meta-analysis from months to days (or even hours!).

Personally, it brought me into an unfamiliar domain with familiar challenges: the need to ensure data accessibility and quality. 
Looking forward to continuing this collaboration and exploring how to make scientific evidence synthesis more efficient and reliable!
