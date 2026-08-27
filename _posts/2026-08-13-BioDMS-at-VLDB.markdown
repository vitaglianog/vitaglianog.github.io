---
lng_pair: id_biodms_vldb_2026
title: Biomedical data management at VLDB 2026
author: Gerardo Vitagliano
category: academic
tags: [academic, workshop, biomedical data, vldb]
img: "/assets/img/thumbs/biodms_thumb.png"
date: 2026-08-13 12:00:00 -0400
published: true
---

<!-- outline-start -->
![](:biodms_banner.png){:style="display: block; margin: auto; width: 100%;"}

We are organizing the first BioDMS workshop at VLDB with the goal of bringing biomedical researchers and data management researchers into the same room.

<!-- outline-end -->

#### Biomedical nails and data-system hammers

Biomedical research is increasingly data-driven, but the data is rarely easy to manage. Researchers and clinicians work with EHR, medical images, genomic measurements, and scientific literature, often with different requirements in terms of quality, privacy constraints, and scale. 
Domain experts understand the scientific questions, while data management researchers build tools for integration, querying, provenance, and reproducibility. Too often, these communities encounter the same problem from different sides without having a place to work on it together.

Almost a year ago, while at SIGMOD 2025, me and [Bojan Karlaš](https://bojan.ninja/) discussed for the need of bringing these communities together. We realized that biomedical researchers have unique data challenges that require specialized solutions, and that data management researchers have tools and techniques that could be adapted to meet those challenges.

Thus, the idea of the [BioDMS](https://biodms.org/) workshop was born. 
After months of brainstorming, planning and coordination, we are excited to present the first edition of the workshop at VLDB 2026!

#### BioDMS 2026

The workshop will take place on September 4th at VLDB 2026 in Boston, from 1:45 PM to 6:15 PM in Grand Ballroom D.
We designed the [program](https://biodms.org/#program) to mix perspectives from biomedical informatics and data systems, with keynotes, invited talks, short presentations of accepted work, a plenary discussion, and a joint poster session.

The response to the first edition was very encouraging.
We received 13 submissions from the biomedical and data management communities, and selected nine for presentation, for an acceptance rate of about 69%.
The submissions included both lightning talks, which introduce a pressing biomedical data problem or an existing tool, and project talks, which propose work-in-progress or future interdisciplinary collaborations.

As we describe in our blog post, [*Data System Hammers for Biomedical Nails*](https://biodms.org/blog/2026/data-system-hammers-for-biomedical-nails/), four themes emerged from the accepted work:

- **Bridging the nail-and-hammer divide.** Some contributions start from a biomedical problem in need of new infrastructure, while others present a data system that can be adapted to a concrete scientific workflow. The program covers examples ranging from MRI data harmonization to cloud-native genomic variant storage and extracting dataset references from biomedical literature.
- **Building a trusted runtime for clinical AI.** Accuracy alone is not enough when an AI system operates in a clinical setting. Several contributions examine hallucinations, provenance, constraints, auditability, and structured execution for agents working with medical data.
- **Scaling to large patient populations.** Population genomics creates storage, indexing, and query-processing problems at a remarkable scale. The accepted work includes systems for querying hundreds of thousands of genomes and techniques for balancing distributed genomic indices.
- **Solving semantic interoperability.** Hospitals and research institutions may adopt the same technical standards and still disagree on the meaning of their data. The workshop will discuss knowledge graphs, multimodal search, metadata harmonization, and shared representations for connecting clinical records, imaging, and genomic data.


#### Keynotes and invited speakers

We are very happy to two keynote speakers and two invited speakers:

- Juliana Freire will open the workshop with *Hammers for Biomedical Nails: From Matching to Meaning in Data Harmonization*.
Her talk will discuss the data harmonization challenges encountered in the ARPA-H Biomedical Data Fabric program and the systems developed to address them.
One aspect I find particularly interesting is the combination of classical algorithms, LLMs, interactive visualization, and human validation.
LLMs can be powerful components, but they do not make the underlying data management problems disappear, especially when semantic ambiguity and differences between institutions require domain expertise.

- Our second keynote will be given by Nils Gehlenborg, whose group develops visual interfaces and computational methods that help scientists and clinicians interact with complex biomedical data.
Their work includes the HubMAP data portal, which supports the discovery and exploration of standardized multimodal spatial and single-cell data.
His perspective brings an important part of the workshop vision into focus: building a technically capable system is not sufficient if researchers cannot effectively explore and use the data it manages.

- Daniel Fabbri will present *Brim: A Democratized AI-Guided Chart Abstraction Platform*.
Brim combines language models with structured review workflows to help experts extract clinical variables from unstructured medical records, while retaining the validation and governance controls required for healthcare data.

- Tim Poterba will present *Embeddable OLAP for Variant Data: Why Warehousing, Search, and Research Can Share an Engine*.
His talk will introduce Phoebe, an embeddable engine built around DataFusion and Vortex for genomic variant warehousing and search.
The system demonstrates how domain-aware analytical infrastructure can avoid expensive exchanges between separate systems and support interactive queries over millions of exomes.

#### Building a community around the problem

The main takeaway from the blog post is that biomedical breakthroughs increasingly depend on our ability to organize, integrate, query, and share large multimodal datasets.
These are not secondary engineering details: they determine whether new scientific methods can be reproduced, deployed, and used across institutions.

Addressing them will require researchers who can bridge biomedical workflows with data quality, storage, integration, and scalable analytics.
Our ambition is therefore for BioDMS to become more than a place where finished work is presented.
We would like it to become a hub for identifying pressing data challenges, an incubator for interdisciplinary projects, and a community that helps train the next generation of biomedical data management researchers.

Many thanks to [Bojan Karlaš](https://bojan.ninja/), [Benjamin Gyori](https://www.khoury.northeastern.edu/people/benjamin-gyori/), and [Ulf Leser](https://www2.informatik.hu-berlin.de/~leser/) for organizing BioDMS with me, as well as to the speakers, authors, reviewers, and sponsors helping us get the community started.

If you are attending VLDB and want to discuss novel data management hammers for biomedical nails, come join us :)
