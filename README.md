# Local Adaptation and Range Expansion in Culex tarsalis: Comparative Genomics and Population-Level Analysis (2021–2022)
***
<p align="center">
<img src="https://user-images.githubusercontent.com/97530809/155350986-35c19f43-21f5-4962-86a7-393d43c75888.png" width="400" height="350">
  </p>

## Project Overview ☰

This project investigates the genomic basis of local adaptation and potential range expansion in *Culex tarsalis*, a principal vector of West Nile virus in North America. Using reference genome analysis, orthogroup identification, gene duplication events, protein function prediction, and population-level sequencing data, the project examines environmental and genetic factors driving divergence among Pacific, Sonoran, and Midwest mosquito populations. Insights aim to inform disease management and anticipate geographic spread.

## Key Takeaways 🔎

       ✓ Completed masking and mappability analysis of the *Cx. tarsalis* reference genome  
       ✓ Identified orthogroups and gene duplication events across multiple Culex species  
       ✓ Annotated protein functions using InterProScan and UniFunc NLP tools  
       ✓ Conducted quality control and alignment of 884 Illumina NGS paired-end samples  
       ✓ Evaluated mapping efficiency pre- and post-genome masking using BWA-MEM  
       ✓ Assessed alternative mapping approaches using Stampy for low-quality reads  
       ✓ Linked orthogroups to Gene Ontology terms for functional analysis  
       ✓ Simplified functional descriptions and visualized frequent terms via word cloud  

## Key Features 🔑

* **Reference Genome Analysis:**

       ✓ Masked repetitive regions with MaskFasta using a custom GFF3 library  
       ✓ Computed genome mappability using GenMap to identify low-complexity regions  
       ✓ Identified orthogroups and inferred gene duplications using OrthoFinder  
       ✓ Constructed rooted species trees with STAG and visualized in Dendroscope  
       ✓ Mapped gene duplications to nodes for Clemson and UC Davis reference genomes  

* **Protein Function Annotation:**

       ✓ Collected predictive protein function data with InterProScan  
       ✓ Combined orthogroup information and functional annotations using SQLite  
       ✓ Simplified protein function descriptions using UniFunc clustering  
       ✓ Created frequency tables and word clouds for common functional terms  

* **NGS Data Processing & Alignment:**

       ✓ Performed quality trimming of 884 Illumina paired-end reads using Trimmomatic  
       ✓ Conducted quality assessment pre- and post-trimming with FastQC  
       ✓ Aligned reads to both unmasked and masked reference genomes using BWA-MEM  
       ✓ Generated alignment statistics with Samtools to evaluate mapping efficiency  
       ✓ Tested alternative alignment using Stampy for divergent or low-quality reads  
       ✓ Filtered 386 high-quality samples for downstream analysis  

* **Comparative Genomics & Functional Analysis:**

       ✓ Mapped gene duplication events to species-specific nodes (Clemson, Davis, N1, C. quinquefasciatus, C. pipiens pallens)  
       ✓ Linked orthogroups to Gene Ontology terms and simplified descriptions  
       ✓ Aggregated annotations to visualize functional patterns across duplicated genes  
       ✓ Created a consolidated orthogroup-to-description table for downstream analysis  

## Visualizations 📶

       ✓ Pre- and post-masking genome mappability distributions  
       ✓ Rooted species tree with annotated gene duplication events  
       ✓ Orthogroup duplication statistics per species and node  
       ✓ Word cloud of most frequent functional annotations  
       ✓ Read mapping statistics before and after genome masking  
       ✓ FastQC per-base sequence quality plots for raw and trimmed data  

## Technologies Used 🛠️

       ✓ Python (Pandas, Matplotlib, NLTK)  
       ✓ Bash / Shell scripting  
       ✓ Bedtools  
       ✓ GenMap  
       ✓ OrthoFinder  
       ✓ Dendroscope  
       ✓ InterProScan  
       ✓ UniFunc  
       ✓ Trimmomatic  
       ✓ FastQC  
       ✓ BWA-MEM  
       ✓ Samtools  
       ✓ Stampy  
       ✓ SQLite / SQLiteStudio  

## Data 📂

* **Source:**  
       ✓ UC Davis Culex tarsalis reference genome (Kern National Wildlife Refuge colony)  
       ✓ Illumina Next-Generation Sequencing paired-end datasets (884 files / 442 pairs)  
       ✓ Comparative protein datasets from *Culex quinquefasciatus* and *Culex pipiens pallens*  

* **Format:**  
       ✓ FASTA, FASTQ, BAM/SAM, TSV/CSV for genome, annotation, and alignment data  
       ✓ GFF3 for repeat annotation  
       ✓ Visual outputs in PNG format for mappability, FastQC, and word clouds  

## License

MIT License  

Copyright (c) 2022 Samantha-A-Taylor
