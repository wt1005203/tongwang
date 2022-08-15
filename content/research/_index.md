---
title: "Research"
date: 2022-08-06T16:47:30.077Z
link: NA
image: /img/organicdevops.webp
description: NA
weight: 10
sitemap:
  priority: 0.6
  weight: 0.5
---

{{< figure src="/research_photos/Interactions_in_MC_schematic.png" width="50%" title="" >}}

Microbial communities are complex due to the multitude of species and diverse types of interactions between them. I am broadly interested in modeling microbial communities with cross-feeding interactions and predator-prey interactions. More specifically, I develop mechanistic models and machine learning methods for solving problems in microbial communities. Motivated by models in statistical physics, math, ecology, epidemiology, and machine learning, I have built computational methods for  
### Prediction of gut fecal metabolite levels from microbial abundance using the ecological model with trophic levels and inference of cross-feeding interactions based on the trophic model
A mechanistic model for the gut microbiome to understand fecal metabolomic profiles?
{{< figure src="/research_photos/trophic_GutCP.png" width="100%" title="" >}}

Following the idea of trophic level in macroecology, we designed a [trophic model](https://journals.plos.org/ploscompbiol/article?id=10.1371/journal.pcbi.1007524) that considers the sequential nutrient consumption and byproduct generation upon consumption. Using a manually-curated database of metabolite-microbe interactions (i.e. consumption or production), our model with four trophic levels generates fecal metabolomic profiles in the best agreement with the real data. Then we wonder if we can improve the prediction performance by adding new interactions or removing existing interactions in mechanistic models. To demonstrate this, we developed the algorithm [GutCP (Gut Cross-feeding Predictor)](https://www.nature.com/articles/s41467-021-21586-6) that leverages the Monte Carlo algorithm to probabilistically search for interactions to add or remove and demonstrated on the trophic model.

### Personalized prediction of metabolomic profiles of human gut microbiomes through deep learning
Personalized prediction of fecal and blood metabolomic profiles based on deep learning methods?
{{< figure src="/research_photos/mNODE.png" width="100%" title="" >}}

Many machine learning methods have been developed to predict fecal and blood metabolomic profiles based on microbiome compositions. However, the current state-of-the-art deep learning methods have not been leveraged. In a [new study](https://www.biorxiv.org/content/10.1101/2022.06.23.497381v1), we proposed a new method — mNODE (Metabolomic profile predictor using Neural Ordinary Differential Equations), based on the state-of-the-art deep neural network models "Neural Ordinary Differential Equations". Our mNODE outperforms existing methods in predicting the metabolomic profiles on both synthetic data and real data such as human gut microbiomes and other natural microbiomes. Further, in the case of human gut microbiomes, mNODE can naturally incorporate dietary information to further enhance the prediction of metabolomic profiles. Finally, we revealed that mNODE can reveal microbe-metabolite interactions.

### Infection dynamics of viruses on the chemotactic bacteria
How do phages infect moving bacteria?
{{< youtube OnPKtrgNocQ >}}

In the past, studies of phage infection in space focused on what happens in bacterial lawns or biofilms. Those studies shed light on how phages attack non-motile bacteria. How do phages infect chemotactic bacteria? To study this question, Derek Ping, an undergraduate student from the lab of [Prof. Seppe Kuehn](https://www.kuehnlab.org/), performed experiments by inoculating the chemotactic E. coli cells together with their phage P1vir at the center of an agar plate with a rich medium (see the YouTube video). In the YouTube video, the outermost bright rings are dense bacterial populations that are migrating at about half a centimeter per hour. However, at the center of the colony, there is a darkened area, about 6cm in diameter, which he showed resulted from the collapse of the bacterial population due to phage lysis. Further, at the center of the colony, we observed a dense region due to the rise of resistant bacteria.

We sought to understand how the phage could create the large central region of the colony where the bacterial population had collapsed. Existing theories based on studies with non-motile bacteria showed that phage could not move over such large distances (centimeters) in such short periods of time (hours) without being actively transported. Therefore, we speculated that the phages travel along with migrating bacteria either during the latent period of infection or while attached to the cell prior to injection. To test this hypothesis, I built a mathematical model that included the ability of phages to “hitchhike” with migrating bacteria. The model confirmed our hypothesis. This study can be found [here](https://www.nature.com/articles/s41396-020-0664-9).

### Other projects
Besides, I studied the ecological and evolutionary dynamics influenced by interactions within microbial communities:
* Functional redundancy in metagenome and metaproteome and how the redundancy difference between two types of data reveals ecological niches and metabolic essentiality.
* Ecological models of microbial exchange of essential nutrients.
* Models of microbial cross-feeding at intermediate scale mediated by carbon sources like acetate and amino acids.
* CRISPR-induced arms-race co-evolution between bacteria and viruses: network structure, prediction of regime shift, and influence of phage migration.

I also worked on COVID-related projects:
* Agent-based model for the University of Illinois at Urbana-Champaign. 
* Data-analysis of internal COVID case data for operational purposes.

<!--
I am interested in developing mechanistic models and machine learning methods for solving problems in microbial communities. Motivated by models in statistical physics, math, ecology, epidemiology, and machine learning, I am broadly interested in modeling microbial communities with cross-feeding interactions and predator-prey interactions. I study the ecological and evolutionary dynamics influenced by those interactions. More specifically, I have worked on
* Functional redundancy in metagenome and metaproteome and how the redundancy difference between two types of data to reveal ecological niches and metabolic essentiality.
* Personalized prediction of metabolomic profiles of human gut microbiomes through deep learning.
* Prediction of gut fecal metabolite levels from microbial abundance using the ecological model with trophic levels.
* Ecological models of microbial exchange of essential nutrients.
* Models of microbial cross-feeding at intermediate scale mediated by carbon sources like acetate and amino acids.
* CRISPR-induced arms-race co-evolution between bacteria and viruses: network structure, prediction of regime shift, and influence of phage migration.
* Infection dynamics of viruses (such as phage P1vir) on the chemotactic bacteria (such as E. colis). 

I also worked on COVID-related projects:
* Agent-based model for the University of Illinois at Urbana-Champaign. 
* Data-analysis of internal COVID case data for operational purposes.
-->

<!-- {{< youtube FizSk5h_akw>}} \-->

<!--

This page represents the landing page for "publications" section. It is also shown under the homepage header for "publications". It should be therefore relatively short and sweet.

\-->