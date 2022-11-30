---
title: "Eliminate false positives in metagenomic profiling based on type IIB restriction sites"
date: 2022-10-25
pubtype: "Preprint"
featured: true
description: "Zheng Sun, Jiang Liu, Meng Zhang, <b>Tong Wang</b>, Shi Huang, Scott T. Weiss, Yang-Yu Liu, <i>bioRxiv, 2022</i>"
tags: #["niche","metaproteome"]
image: #"/img/organicdevops.webp"
link: "https://www.biorxiv.org/content/10.1101/2022.10.24.513546v1.abstract"
fact: "Interesting little tidbit shown below image on summary and detail page"
weight: 400
sitemap:
  priority : 0.8
---

Accurate species identification and abundance estimation are critical for the interpretation of whole metagenome shotgun sequencing (WMS) data. Numerous computational methods, broadly referred to as metagenomic profilers, have been developed to identify species in microbiome samples by classification of sequencing reads and quantification of their relative abundances. Yet, existing metagenomic profilers typically suffer from false positive identifications and consequently biased relative abundance estimation (as false positives can be accounted for more than 90% of total identified species). Here, we present a new metagenomic profiler MAP2B (MetAgenomic Profiler based on type IIB restriction site) to resolve those issues. We first illustrate the pitfalls of using relative abundance as the only feature in determining false positives. We then propose a feature set to distinguish false positives from true positives. By benchmarking the performance in metagenomic profiling using data from CAMI2 (Critical Assessment of Metagenome Interpretation: second round of challenge), we illustrate the superior performance of MAP2B (F1 score ~ 0.93) over existing metagenomic profilers (F1 score ranges from 0.18 to 0.58). We further tested the performance of MAP2B using real WMS data from an ATCC mock community, confirming its superior performance and robustness against sequencing depth. In addition, by leveraging WMS data from an IBD cohort, we demonstrate the taxonomic features obtained by MAP2B can better discriminate disease status and predict metabolomic profiles.