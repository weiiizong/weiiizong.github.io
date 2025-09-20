---
layout: archive
title: "Research"
permalink: /research/
author_profile: true
---

# 1. Statistical Methodology
## 1.1. Cross-species congruence analysis

Model organisms are instrumental substitutes for human studies to expedite basic, translational, and clinical research. Despite their indispensable role in mechanistic investigation and drug development, molecular congruence of animal models to human has long been questioned and debated. We have developed a framework, namely Congruence Analysis for Model Organisms (CAMO) [1], using a threshold-free Bayesian differential expression analysis to avoid the subjective p-value cutoff and quantitative concordance/discordance scores based on F-measure from machine learning perspective to numerically quantify the congruence level. The downstream analyses of this framework utilize pathwaycentric downstream investigation, knowledge retrieval by text mining and community detection algorithm in pathway topological structure to provide foundations for biological hypothesis generation.

To facilitate interdisciplinary research, we also provided a web-based tool by R Shiny to interactively implement the streamlined workflow and visualize the congruence level at both genome-wide and pathway specific levels. It has a graphical user interface (GUI) for better visualization of the results and is easy to implement without requiring any R programming knowledge.


### Publication
[1] **Wei Zong**, Tanbin Rahman, Li Zhu, Xiangrui Zeng, Yingjin Zhang, Jian Zou, Song Liu, Zhao Ren, Jingyi Jessica Li, Etienne Sibille, Adrian V. Lee, Steffi Oesterreich, Tianzhou Ma and George C. Tseng. (2023) Transcriptomic congruence analysis for evaluating model organisms. _Proceedings of the National Academy of Sciences_. 120(6):e2202584120. 

## 1.2. High-dimensional clustering

Unsupervised clustering analysis has been widely applied directly on high-dimensional omics data to identify homogeneous groups such that samples within a group share some common attributes. However, due to the data complexity with multifaceted information, multiple plausible sample partitions may coexist, while conventional clustering methods typically yield only one clustering solution, limiting their capacity to fully capture all facets of cluster structures in high-dimensional data. To address this, I developed a multifacet clustering method (MFClust) that simultaneously identifies feature assignments and sample clusters, uncovering complex biological patterns often overlooked by traditional approaches [2]. This method is particularly valuable in contexts where multiple clustering solutions correspond to different aspects of the underlying biological processes.

One prominent application of clustering analysis is disease subtyping, aimed at identifying patient subgroups with differential disease progression, prognosis, or treatment response, as an essential step towards precision medicine. To ensure clinical relevance of the identified clusters, I am developing a multivariate clinical variable guided subtyping model to (mg-Clust) to identify molecular subtypes that are associated with multiple disease-related clinical variables collectively. It is a unified generative model where the disease subtyping model and multivariate clinical variable association model interact with each other through a latent subtyping variable. This paper is in preparation [3].


In conventional differential analysis pipeline, pathway enrichment analysis provides a knowledge-driven approach to interpret differentially expressed genes associated with disease status. However, when multiple studies of different conditions are jointly analyzed, novel integrative tools are needed. In addition, pathway redundancy introduced by combining multiple public pathway databases hinders interpretation and knowledge discovery. We have developed a meta-analytical tool, Comparative Pathway Integrator (CPI), to address this using adaptively weighted Fisher’s method to discover consensual and differential enrichment patterns, a tight clustering algorithm to reduce pathway redundancy, and a text mining algorithm to assist interpretation of the pathway clusters [4].

### Highlight Publication
[2] **Wei Zong**, Danyang Li, Marianne Seney, Colleen McClung, George C. Tseng. (2024) Model-based multi-facet clustering with high-dimensional omics applications. _Biostatistics_.

[3] Yujia Li^, Liu Peng^, Wenjia Wang^, **Wei Zong**, Yusi Fang, Zhao Ren, Lu Tang, Juan Celedon, Steffi Oesterreich, and George C Tseng. (2024) Outcome-guided disease subtyping by generative model
and weighted joint likelihood in transcriptomic applications. _Annals of Applied Statistics_.

[4] **Wei Zong**^, Danyang Li^, Lu Tang, George C. Tseng. (2025+) Multivariate guided disease subtyping for high-dimensional omics data. _In preparation_.

[5] Xiangrui Zeng^, **Wei Zong**^, Chien-Wei Lin, Zhou Fang, Tianzhou Ma, David A Lewis, John F Enwright, George C. Tseng. (2020) Comparative Pathway Integrator: a framework of meta-analytic integration of multiple transcriptomic studies for consensual and differential pathway analysis.  _Genes (2020)_.



## 1.3. Circadian analysis
Circadian rhythms are 24-hour oscillations of behavioral and biological processes that adapt life to the diurnal daylight cycle. The disruption of the molecular circadian rhythms is associated with the development of various psychiatric diseases and thus there is increasing interest in circadian studies to reveal molecular mechanisms of rhythm-related physiological processes and disease etiology. Cosinor model is one of the most popular approaches for molecular circadian rhythm analysis which assumes the expression level of a gene is a sinusoidal function of the circadian time. However, due to the complexity of the non-linear relationship, circadian detection power calculation is usually achieved through a timeconsuming Monte-Carlo simulation (MC). I have developed an analytical method, namely CircaPower, to perform fast and accurate circadian power analysis [5]. When a contrasting condition exists, differential circadian analysis can be used to investigate if the condition shift is associated with rhythm disruption. A systematic workflow (DiffCircaPipeline) has been proposed to detect multifaceted differential circadian
characteristics including phase, amplitude, and rhythm fitness [6].

### Publication
[5] **Wei Zong**, Marianne L. Seney, Kyle D. Ketchesin, Michael T. Gorczyca, Andrew C. Liu, Karyn A. Esser, George C. Tseng, Colleen A. McClung and Zhiguang Huo. (2023) Experimental design and power calculation in omics circadian rhythmicity detection. _Statistics in Medicine_.

[6] Xiangning Xue, **Wei Zong**, Zhiguang Huo, Kyle D. Ketchesin, Madeline R. Scott, Kaitlyn A. Petersen,
RyanW. Logan, Marianne L. Seney , Colleen McClung and George Tseng. (2023) DiffCircaPipeline: A framework for multifaceted characterization of differential rhythmicity. _Bioinformatics_.


# Interdisciplinary Application
My collaborative work focuses on investigating the molecular circadian rhythm shift in different psychiatric disorders (e.g., bipolar disorder, major depression, drug addiction, etc.), gender groups, and brain regions. We have explored the effects of psychosis and schizophrenia on circadian patterns of gene expression in the human striatum [7, 8] and prefrontal cortex [9] respectively using RNA-seq data from postmortem samples. We investigated the molecular rhythms across the three striatal subregions (caudate, putamen, and nucleus accumbens) in the human dorsal and ventral striatum, which establishes a temporal map of rhythms across the human striatum and helps in understanding how disruption could lead to pathology [10]. For drug addiction, we studied the molecular circadian disruption in people with opioid use disorder using postmortem samples in the two key brain areas associated with dysfunction of activity in corticostriatal circuits (prefrontal cortex and nucleus accumbens) [11]. Besides human studies, I am also working on multiple mouse datasets to investigate molecular rhythms in different neuron cell types including astrocyte, D1, D2 and homogenate [12, 13, 14].

### Highlight Publication
[7] Kyle D Ketchesin^, **Wei Zong**^, Mariah A Hildebrand, Madeline R Scott, Marianne L Seney, Kelly M Cahill, Vaishnavi G Shankar, Jill R Glausier, David A Lewis, George C Tseng, Colleen A McClung. (2023) Diurnal alterations in gene expression across striatal subregions in psychosis. _Biological Psychiatry_.

[8] Megan S Perez, RuoFei Yin, Madeline R Scott, **Wei Zong**, Marianne L Seney, Xiangning Xue, Mariah A Hildebrand, Vaishnavi G Shankar, Jill R Glausier, David A Lewis, George C. Tseng, Kyle D. Ketchesin, Colleen A. McClung. Sex and regional differences in gene expression across the striatum in psychosis. _Translational Psychiatry_.

[9] Marianne L Seney, Kelly Cahill, John F Enwright, Ryan W Logan, Zhiguang Huo, **Wei Zong**, George Tseng, Colleen A McClung. (2019) Diurnal rhythms in gene expression in the prefrontal cortex in schizophrenia. _Nature Communications_.

[10] Kyle D Ketchesin^, **Wei Zong**^, Mariah A Hildebrand, Marianne L Seney, Kelly M Cahill, Madeline R Scott, Vaishnavi G Shankar, Jill R Glausier, David A Lewis, George C Tseng, Colleen A McClung. (2021) Diurnal rhythms across the human dorsal and ventral striatum. _Proceedings of the National Academy of Sciences_.

[11] Xiangning Xue, **Wei Zong**, Jill R Glausier, Sam-Moon Kim, Micah A Shelton, BaDoi N Phan, Chaitanya Srinivasan, Andreas R Pfenning, George C Tseng, David A Lewis, Marianne L Seney, RyanWLogan. (2022) Molecular rhythm alterations in prefrontal cortex and nucleus accumbens associated with opioid use disorder. _Translational Psychiatry_.

[12] Lauren M. DePoy, Kaitlyn A. Petersen, **Wei Zong**, Kyle D. Ketchesin, Ross C. Matthaei, RuoFei Yin, Megan S. Perez, Chelsea A. Vadnie, Darius Becker-Krail, Madeline R. Scott, George C Tseng, Colleen A. McClung. (2024) Cell-type and sex-specific rhythmic gene expression in the nucleus accumbens. _Molecular Psychiatry_.

[13] Kaitlyn A Petersen, **Wei Zong**, Lauren M Depoy, Madeline R Scott, Vaishnavi G Shankar, Jennifer N Burns, Allison J Cerwensky, Sam-Moon Kim, Kyle D Ketchesin, George C Tseng, Colleen A McClung. (2024) Comparative rhythmic transcriptome profiling of human and mouse striatal subregions. _Neuropsychopharmacology_.

[14] Darius D Becker-Krail, Kyle D Ketchesin, Jennifer N Burns, **Wei Zong**, Mariah A Hildebrand, Lauren M DePoy, Chelsea A Vadnie, George C Tseng, Ryan W Logan, Yanhua H Huang, Colleen A McClung. (2022) Astrocyte Molecular Clock Function in the Nucleus Accumbens is Important for Reward-Related Behavior. _Biological Psychiatry_.
