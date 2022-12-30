---
layout: archive
title: "Research"
permalink: /research/
author_profile: true
---

# 1. Statistical Methodology
## 1.1. Cross-species congruence evaluation
### Past and on-going research

Model organisms are instrumental substitutes for human studies to expedite basic, translational, and clinical research. Despite their indispensable role in mechanistic investigation and drug development, molecular congruence of animal models to human has long been questioned and debated. We have developed a framework, namely Congruence Analysis for Model Organisms (CAMO) [1], using a threshold-free Bayesian differential expression analysis to avoid the subjective p-value cutoff and quantitative concordance/discordance scores based on F-measure from machine learning perspective to numerically quantify the congruence level. The downstream analyses of this framework utilize pathwaycentric downstream investigation, knowledge retrieval by text mining and community detection algorithm in pathway topological structure to provide foundations for biological hypothesis generation.

To facilitate interdisciplinary research, we also provided a web-based tool by R Shiny to interactively implement
the streamlined workflow and visualize the congruence level at both genome-wide and pathwayspecific
levels. It has a graphical user interface (GUI) for better visualization of the results and is easy to
implement without requiring any R programming knowledge.


### Publication
[1] **Wei Zong**, Tanbin Rahman, Li Zhu, Xiangrui Zeng, Yingjin Zhang, Jian Zou, Song Liu, Zhao Ren, Jingyi Jessica Li, Etienne Sibille, Adrian V. Lee, Steffi Oesterreich, Tianzhou Ma and George C. Tseng. Transcriptomic congruence analysis for evaluating model organisms. _Accepted at Proceedings of the National Academy of Sciences_.

## 1.2. High-dimensional clustering
### Past and on-going research

Pathway enrichment analysis provides a knowledge-driven approach to interpret differentially expressed genes associated with disease status. However, when multiple studies of different conditions are jointly analyzed, novel integrative tools are needed. In addition, pathway redundancy introduced by combining multiple public pathway databases hinders interpretation and knowledge discovery. We have developed a meta-analytical tool, Comparative Pathway Integrator (CPI), to address this using adaptively weighted Fisher’s method to discover consensual and differential enrichment patterns, a tight clustering algorithm to reduce pathway redundancy, and a text mining algorithm to assist interpretation of the pathway clusters [2].

Unsupervised clustering analysis has also been widely applied directly on high-dimensional omics data to identify homogeneous groups such that samples within a group share some common attributes. One prominent application of clustering analysis is disease subtyping, aimed at identifying patient subgroups with differential disease progression, prognosis, or treatment response, as an essential step towards precision medicine. However, conventional unsupervised clustering methods are highly exploratory and often fail to identify clinically actionable subtypes due to the multifaceted information contained within high-dimensional data. I have developed a multivariate clinical variable guided subtyping model to (mg-Clust) to identify molecular subtypes that are associated with multiple disease-related clinical variables collectively. It is a unified generative model where the disease subtyping model and multivariate clinical variable association model interact with each other through a latent subtyping variable. A hybrid of group lasso and elastic net penalties facilitates the selection of effective genes and clinical variables toward clinically meaningful cluster construction. This paper is preparing for submitting to Bioinformatics [3].

Another approach to explore the multifaceted information in omics data is to consider alternative clustering solutions. I am working on a model-based multiple clustering model aimed at identifying multiple high-quality clustering solutions simultaneously to encourage knowledge discovery.

### Publication
[2] Xiangrui Zeng^, **Wei Zong**^, Chien-Wei Lin, Zhou Fang, Tianzhou Ma, David A Lewis, John F Enwright, George C. Tseng. Comparative Pathway Integrator: a framework of meta-analytic integration of multiple transcriptomic studies for consensual and differential pathway analysis. _Genes (2020)_.
[3] **Wei Zong**, Lu Tang, George C. Tseng. Multivariate guided disease subtyping for high-dimensional omics data. _Ready to submit_.

## 1.3. Circadian analysis
### Past and on-going research
Circadian rhythms are 24-hour oscillations of behavioral and biological processes that adapt life to the diurnal daylight cycle. The disruption of the molecular circadian rhythms is associated with the development of various psychiatric diseases and thus there is increasing interest in circadian studies to reveal molecular mechanisms of rhythm-related physiological processes and disease etiology. Cosinor model is one of the most popular approaches for molecular circadian rhythm analysis which assumes the expression level of a gene is a sinusoidal function of the circadian time. However, due to the complexity of the non-linear relationship, circadian detection power calculation is usually achieved through a timeconsuming Monte-Carlo simulation (MC). I have developed an analytical method, namely CircaPower, to perform fast and accurate circadian power analysis [4]. When a contrasting condition exists, differential circadian analysis can be used to investigate if the condition shift is associated with rhythm disruption. A systematic workflow (DiffCircaPipeline) has been proposed to detect multifaceted differential circadian
characteristics including phase, amplitude, and rhythm fitness [5].

### Publication
[4] **Wei Zong**, Marianne L. Seney, Kyle D. Ketchesin, Michael T. Gorczyca, Andrew C. Liu, Karyn A. Esser, George C. Tseng, Colleen A. McClung and Zhiguang Huo. Experimental design and power calculation in omics circadian rhythmicity detection. _Submitted to Statistics in Medicine_.

[5] Xiangning Xue, **Wei Zong**, Zhiguang Huo, Kyle D. Ketchesin, Madeline R. Scott, Kaitlyn A. Petersen,
RyanW. Logan, Marianne L. Seney , Colleen McClung and George Tseng. DiffCircaPipeline:
A framework for multifaceted characterization of differential rhythmicity. _Accepted at Bioinformatics_.


# Bioinformatics Application
### Past and on-going research
My collaborative work focuses on investigating the molecular circadian rhythm shift in different psychiatric disorders (e.g., bipolar disorder, major depression, drug addiction, etc.), gender groups, and brain regions. We have explored the effects of psychosis and schizophrenia on circadian patterns of gene expression in the human striatum [6] and prefrontal cortex [7] respectively using RNA-seq data from postmortem samples. We investigated the molecular rhythms across the three striatal subregions (caudate, putamen, and nucleus accumbens) in the human dorsal and ventral striatum, which establishes a temporal map of rhythms across the human striatum and helps in understanding how disruption could lead to pathology [8]. For drug addiction, we studied the molecular circadian disruption in people with opioid use disorder using postmortem samples in the two key brain areas associated with dysfunction of activity in corticostriatal circuits (prefrontal cortex and nucleus accumbens) [9]. Besides human studies, I am also working on multiple mouse datasets to investigate molecular rhythms in different neuron cell types including astrocyte [10], D1, D2 and homogenate.

### Publication
[6] Kyle D Ketchesin^, **Wei Zong**^, Mariah A Hildebrand, Madeline R Scott, Marianne L Seney, Kelly M Cahill, Vaishnavi G Shankar, Jill R Glausier, David A Lewis, George C Tseng, Colleen A McClung. Diurnal alterations in gene expression across striatal subregions in psychosis. _Biological Psychiatry (2022)_.

[7] Marianne L Seney, Kelly Cahill, John F Enwright, Ryan W Logan, Zhiguang Huo, **Wei Zong**, George Tseng, Colleen A McClung. Diurnal rhythms in gene expression in the prefrontal cortex in schizophrenia. _Nature Communications (2019)_.
[8] Kyle D Ketchesin^, **Wei Zong**^, Mariah A Hildebrand, Marianne L Seney, Kelly M Cahill, Madeline R Scott, Vaishnavi G Shankar, Jill R Glausier, David A Lewis, George C Tseng, Colleen A McClung. Diurnal rhythms across the human dorsal and ventral striatum. _Proceedings of the National Academy of Sciences (2021)_.

[9] Xiangning Xue, **Wei Zong**, Jill R Glausier, Sam-Moon Kim, Micah A Shelton, BaDoi N Phan, Chaitanya Srinivasan, Andreas R Pfenning, George C Tseng, David A Lewis, Marianne L Seney, RyanWLogan. Molecular rhythm alterations in prefrontal cortex and nucleus accumbens associated with opioid use disorder. _Translational Psychiatry (2022)_.

[10] Darius D Becker-Krail, Kyle D Ketchesin, Jennifer N Burns, **Wei Zong**, Mariah A Hildebrand, Lauren M DePoy, Chelsea A Vadnie, George C Tseng, Ryan W Logan, Yanhua H Huang, Colleen A McClung. Astrocyte Molecular Clock Function in the Nucleus Accumbens is Important for Reward-Related Behavior. _Biological Psychiatry (2022)_.
