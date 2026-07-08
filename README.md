# Cows-and-Goats-Microbiome-Data-Analysis
This repository contains the scripts and input data for the biostatistical analysis used in:

Corral-Jara et al.
"Species-specific rumen microbial responses to dietary inhibition of methanogenesis in cows and goats"

## Data availability

Raw sequencing data are available at NCBI Sequence Read Archive:

PRJNA762012

## Workflow

The analysis consists of five main steps:

1. Differential occurrence analysis (DESeq2)
2. Co-occurrence network construction (ccrepe)
3. Cluster identification (K-means)
4. KEGG pathway integration (KEGGREST)
5. PLS analyses and variable selection (mixOmics)

## Software

Analyses were performed in:

- R version 4.4.1.
- DESeq2
- ccrepe
- igraph
- mixOmics
- KEGGREST
- dplyr
- plyr
- data.table


## Input files

The following files are required:

- BGI_vaches_RNA_seq.csv
- OTUs_vaches.csv
- coldata_vaches.csv
- metabolites.csv
- CH4.csv
- CH4_milk.csv
- CH4_FPCM.csv
- CH4_MSI.csv
- CH4_CO2.csv

## Output files

- deKOs_COS_CTL.csv
- deOTUs_COS_CTL.csv
- network_edges.csv
- kmeans_clusters.csv
- PLS_loadings.csv






