# in-host-Mtbc-dynamics
This repository contains the Jupyter Notebooks used for data processing and analysis for the article “In-host population dynamics of *Mycobacterium tuberculosis* complex during active disease” (Vargas et al. 2021, https://elifesciences.org/articles/61805). Notebooks were run in order from top to bottom as listed below. All code was written in Python 2 and running code within these notebooks requires installing the necessary python packages, bioinformatics pipelines & changing the directory paths within the notebooks.

* (A) Find Genomic Coordinates for Epitope Peptide Sequences using BLAST
* (B) Create Gene Categories

  * Replicate Isolates/(A) Process Replicate Samples - FASTQ to VCF
  * Replicate Isolates/(B) Process Replicate Samples – Run Kraken on FASTQ

  * Longitudinal Isolates/(A) Process Longitudinal Samples - FASTQ to VCF
  * Longitudinal Isolates/(B) Process Longitudinal Samples – Run Kraken on FASTQ

* (C) Process Replicate and Longitudinal Samples – Depth Extraction at Lineage Defining SNP sites for F2 Mixed Measure
* (D) Filter Replicate and Longitudinal Samples – Contamination with Kraken and F2 Mixed Measure
* (E) Process Replicate and Longitudinal Samples – Collect SNV Calls with Differing Alt AF between Sample Pairs
* (F) Code to Functionally Annotate Single Nucleotide Variants
* (G) PacBio Illumina Comparison - Empirical Base Pair Recall Score Positions to Drop
* (H) Filter Replicate and Longitudinal Samples – Contamination with Fixed SNP Threshold

  * Replicate Isolates/(C) Retrieve SNPs between Replicate Pairs with AF change of 25% or more

  * Longitudinal Isolates/(C) Retrieve SNPs between Longitudinal Pairs with AF change of 25% or more

* (I) Replicate and Longitudinal SNP comparison to find optimal AF change threshold% for in-host SNPs

  * Longitudinal Isolates/(D) Retrieve SNPs between Longitudinal Pairs with AF change of 5% or more
  * Longitudinal Isolates/(E) Retrieve SNPs between Longitudinal Pairs with AF change of 70% or more

   * Longitudinal Isolates/In-host SNPs with AF change of 70% analyses/(A) Organize and Visualize SNPs with Circos Plot and Heatmap
   * Longitudinal Isolates/In-host SNPs with AF change of 70% analyses/(B) Mutational Spectrum of SNPs and AF change between Functional SNP type
   * Longitudinal Isolates/In-host SNPs with AF change of 70% analyses/(C) Nucleotide Diversity across Gene Categories and Epitopes
   * Longitudinal Isolates/In-host SNPs with AF change of 70% analyses/(D) Num SNPs vs Time Between Sample Collection
   * Longitudinal Isolates/In-host SNPs with AF change of 70% analyses/(E) Num SNPs vs Time Between Sample Collection for Confirmed Failure Relapse Patients
   * Longitudinal Isolates/In-host SNPs with AF change of 70% analyses/(F) Convergent Mutations at Pathway Level Analysis
   
  * Longitudinal Isolates/(F) Num Heterozygous SNPs in First vs Second Sample in Treatment Failure Patients
  * Longitudinal Isolates/(G) Drug Resistance Genotype Prediction on Longitudinal Samples
  * Longitudinal Isolates/(H) Antibiotic Resistance Allele Dynamics
  * Longitudinal Isolates/(I) Antibiotic Resistance Allele Dynamics for Confirmed Failure Relapse Patients
  * Longitudinal Isolates/(J) Analyses on Time between Sampling for Mixed, Reinfection and Persistent Infections

  * Short Read Simulations/(A) Mtb Genome (gene-length) Complete Genome to H37Rv Mapping Assessment
  * Short Read Simulations/(B) Simulate Reads from Complete Genomes
  * Short Read Simulations/(C) Call Variants in Reference Genomes and Simulated Samples against H37Rv
  * Short Read Simulations/(D) Analysis of Variant Calls from Simulated Reads

  * SNPs from Public Samples & tSNE Homoplasy Visualization/(A) Scraping Public WGS Samples for Constructing Genotypes Matrix
  * SNPs from Public Samples & tSNE Homoplasy Visualization/(B) Assign Lineages to Samples, Downsample & Re-Filter for Genotypes Matrix
  * SNPs from Public Samples & tSNE Homoplasy Visualization/(C) Construct Pairwise SNP Distance Matrix from Genotypes Matrix
  * SNPs from Public Samples & tSNE Homoplasy Visualization/(D) Phylogenetic Convergence Test in Public Samples for In-Host SNPs
  * SNPs from Public Samples & tSNE Homoplasy Visualization/(E) t-SNE on Pairwise SNP Distance Matrix
  * SNPs from Public Samples & tSNE Homoplasy Visualization/(F) t-SNE SNV Homoplasy Visualization
