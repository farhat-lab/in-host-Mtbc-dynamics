# in-host-Mtbc-dynamics
This repository contains the Jupyter Notebooks used for data processing and analysis for the article “In-host population dynamics of *Mycobacterium tuberculosis* complex during active disease” (Vargas et al. 2021, https://elifesciences.org/articles/61805). Notebooks were run in order from top to bottom as listed below. All code was written in Python 2 and running code within these notebooks requires installing the necessary python packages, bioinformatics pipelines & changing the directory paths within the notebooks.

(A) Find Genomic Coordinates for Epitope Peptide Sequences using BLAST
(B) Create Gene Categories

Replicate Isolates/
* (A) Process Replicate Samples - FASTQ to VCF
* (B) Process Replicate Samples – Run Kraken on FASTQ

Longitudinal Isolates/
* (A) Process Longitudinal Samples - FASTQ to VCF
* (B) Process Longitudinal Samples – Run Kraken on FASTQ

(C) Process Replicate and Longitudinal Samples – Depth Extraction at Lineage Defining SNP sites for F2 Mixed Measure
(D) Filter Replicate and Longitudinal Samples – Contamination with Kraken and F2 Mixed Measure
(E) Process Replicate and Longitudinal Samples – Collect SNV Calls with Differing Alt AF between Sample Pairs
(F) Code to Functionally Annotate Single Nucleotide Variants
(G) PacBio Illumina Comparison - Empirical Base Pair Recall Score Positions to Drop
(H) Filter Replicate and Longitudinal Samples – Contamination with Fixed SNP Threshold

Replicate Isolates/
* (C) Retrieve SNPs between Replicate Pairs with AF change of 25% or more

Longitudinal Isolates/
* (C) Retrieve SNPs between Longitudinal Pairs with AF change of 25% or more

(I) Replicate and Longitudinal SNP comparison to find optimal AF change threshold% for in-host SNPs

Longitudinal Isolates/
* (D) Retrieve SNPs between Longitudinal Pairs with AF change of 5% or more
* (E) Retrieve SNPs between Longitudinal Pairs with AF change of 70% or more

* In-host SNPs with AF change of 70% analyses/
 * (A) Organize and Visualize SNPs with Circos Plot and Heatmap
 * (B) Mutational Spectrum of SNPs and AF change between Functional SNP type
 * (C) Nucleotide Diversity across Gene Categories and Epitopes
 * (D) Num SNPs vs Time Between Sample Collection
 * (E) Num SNPs vs Time Between Sample Collection for Confirmed Failure Relapse Patients
 * (F) Convergent Mutations at Pathway Level Analysis

* (F) Num Heterozygous SNPs in First vs Second Sample in Treatment Failure Patients
* (G) Drug Resistance Genotype Prediction on Longitudinal Samples
* (H) Antibiotic Resistance Allele Dynamics
* (I) Antibiotic Resistance Allele Dynamics for Confirmed Failure Relapse Patients
* (J) Analyses on Time between Sampling for Mixed, Reinfection and Persistent Infections

Short Read Simulations/
* (A) Mtb Genome (gene-length) Complete Genome to H37Rv Mapping Assessment
* (B) Simulate Reads from Complete Genomes
* (C) Call Variants in Reference Genomes and Simulated Samples against H37Rv
* (D) Analysis of Variant Calls from Simulated Reads

SNPs from Public Samples & tSNE Homoplasy Visualization/
* (A) Scraping Public WGS Samples for Constructing Genotypes Matrix
* (B) Assign Lineages to Samples, Downsample & Re-Filter for Genotypes Matrix
* (C) Construct Pairwise SNP Distance Matrix from Genotypes Matrix
* (D) Phylogenetic Convergence Test in Public Samples for In-Host SNPs
* (E) t-SNE on Pairwise SNP Distance Matrix
* (F) t-SNE SNV Homoplasy Visualization

