---
lng_pair: id_duckdb_pollock
title: DuckDB meets Pollock
author: Gerardo Vitagliano
category: academic
tags: [academic, pollock, duckdb, csv]
img: "/assets/img/posts/pollock_duckdb.jpg"
date: 2025-04-16 10:00:00 -0400
published: true
---

<!-- outline-start -->

The DuckDB team used Pollock to test and improve its CSV reader on messy, real-world files.

<!-- outline-end -->

#### From research to industry 

Research projects often end with a paper, an artifact, and the hope that someone will eventually find them useful. It is therefore particularly satisfying to see a project being picked up by people who build a widely used system.

[Pollock](https://www.vldb.org/pvldb/vol16/p1870-vitagliano.pdf) is a benchmark for testing how reliably data systems load non-standard CSV files. It is based on the kinds of structural and dialect errors that appear in hundreds of thousands of files in the wild, including inconsistent rows, unusual delimiters, multiple headers, and incorrect quoting.

#### Into the CSV abyss

Pedro Holanda and Gábor Szárnyas from DuckDB added the system to the benchmark and used the results to examine its CSV reader in detail. With the benchmark configuration, DuckDB correctly read 99.61% of the generated data and reached the highest weighted Pollock score among the evaluated systems.

The interesting part is not only the ranking. The benchmark gave the team a reproducible way to inspect failure modes and improve the behavior of the parser on difficult files. That is exactly the kind of practical feedback loop we hoped Pollock could enable.

I collaborated with Pedro and Gábor on the resulting DuckDB article, [Into the CSV Abyss](https://duckdb.org/2025/04/16/duckdb-csv-pollock-benchmark). Props also go to my Pollock coauthors Mazhar Hameed, Lan Jiang, Lucas Reisener, Eugene Wu, and Felix Naumann. It is great to see our research being employed by industry leaders!
