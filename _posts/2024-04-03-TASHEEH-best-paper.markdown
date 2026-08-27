---
lng_pair: id_tasheeh_best_paper
title: TASHEEH wins the EDBT Best Paper Award
author: Gerardo Vitagliano
category: academic
tags: [academic, data preparation, csv, award]
img: "/assets/img/posts/tasheesh_1.png"
date: 2024-04-03 12:00:00 +0200
published: true
---

<!-- outline-start -->

Our paper on repairing malformed rows in raw CSV files received the EDBT 2024 Best Paper Award!

<!-- outline-end -->

#### Repairing the structure of messy files

If you have previously heard my research pitch, you know that CSV looks like a very simple format, but real files have a talent for breaking simple assumptions. 
These problems have been at the center of my [PhD thesis](https://hpi.de/en/database-group/projects/data-integration-projects/data-preparation/).
Rows can have missing or additional fields, quotes can be inconsistent, and metadata can appear where a parser expects a table. Before we can clean the values in such a file, we first have to recover its structure.

In [TASHEEH](https://openproceedings.org/2024/conf/edbt/paper-108.pdf), we study how to repair malformed rows by learning from the dominant patterns in the file itself. The system identifies structurally inconsistent records, aligns them with well-formed patterns, and applies transformations that bring the rows back into a consistent shape.

#### A very welcome recognition

I am very honored that this work received the [EDBT 2024 Best Paper Award](https://dastlab.github.io/edbticdt2024/?contents=awards_bp_edbt.html). The paper was led by Mazhar Hameed, and we worked together with Fabian Panse and Felix Naumann, and it grew out of a longer line of research on making messy files usable without asking people to repair every corner case by hand.

More than the award itself, I am happy that data preparation research is gaining attention. File repair may not be the most glamorous step of a data pipeline, but nothing downstream works particularly well if the data cannot be loaded correctly in the first place!
