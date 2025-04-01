---
title: Notes in seminar—"Spatial organization of gliomas and head & neck cancer"
author: wenzy
date: 2025-04-01 18:46:22 +0800
categories: [Seminar]
tags: [notes, woolgathering]
math: true
mermaid: true
pin: false
---

## Seminar information

### Speaker

- Name: [Itay Tirosh](https://scholar.google.com.hk/citations?hl=zh-CN&user=56gr8ZMAAAAJ)

- Institution: Weizmann Institute of Science

### Oragnization

- TICSSO

## Thoughts

The talk was tightly associated with one of my fellows’ work, and potentially would also be associated with mine in the future. There was much unpublished data, so I can’t simply post the slides. 

The topic was about tumour heterogeneity. Compared to other studies that involved spatial transcriptomics, Tirosh had a different perspective when it came to cell-type annotation mixtures in some slides. And based on the structured / mixed / disorganized sample slides, his group devised a coherent score to understand the spot-spot neighbouring structures and their corresponding relations with specific cell types. The emergence of this thinking was very much relied on the inherent characteristics of spatial transcriptome data - each spot has its own imputed cell types and fixed neighbours, and whether the cell-type-coherency between each spot and its neighbouring spots is determined by the cell type within each spot is a very natural inference. 

However, most slides I used to see mainly belonged to Tirosh’s “structured” category. I wonder why I didn’t see other types of slides before, as I’ve never truly accessed spatial data. So, I asked my fellow who has been working on spatial data for several months, and he told me that the other types would be considered “bad”, and would sometimes be dropped. Examining data without bias is essential for discovering more interesting biological phenomena.

Another enlightenment I got was from the second research he introduced. When they categorized spatial zones, they also checked the distribution of different cell types along with these zones. They didn’t rush to a conclusion about the distributions, but separated sample by sample in analysing the cell type of their interest. Then, two entirely separated distributions were exposed, which were formerly averaged in the mixed overall distribution. And these two groups also happened to align with a typical clinical difference in that cancer type. This reminded me of “Simpson's paradox” I heard in the conference held by CCBSB in 2023:

> Simpson's paradox is a phenomenon in probability and statistics in which a trend appears in several groups of data but disappears or reverses when the groups are combined.

It's hard to guess how much effort they’ve put into observing and dividing different distributions. But it really helped to reveal the true meaning of data, which might be closer to the real phenomenon with biological significance we would like to explore. 

These two insights really touched me. Bioinformatics is never running pipelines and throwing useless figures just to look fancy. I shall be meticulous in observing data in **each** step, even if the processing procedures seem mature and fixed, especially when dealing with datasets originally from complex sources. 

In the era of “multi-omics”, we tend to pursue a seemingly consistent, comprehensive, and integral combination of omics data. And confronting tedious co-op tasks with pipelines to serve an existing hypothesis, it may be easy to lose the sensitivity of dissecting differences in analysing processes. This seminar was like another reminder to me about what is **data-driven**, and what bioinformatics can truly do. 
