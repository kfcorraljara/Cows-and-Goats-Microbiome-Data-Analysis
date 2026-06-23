# Cows-and-Goats-Microbiome-Data-Analysis
This repository contains the scripts used in:

Corral-Jara et al.
"Species-specific rumen microbial responses to dietary inhibition of methanogenesis in cows and goats"


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

Package versions are reported in:

sessionInfo.txt

## Input files

The following files are required:

data/

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

results/

- deKOs_COS_CTL.csv
- deOTUs_COS_CTL.csv
- network_edges.csv
- kmeans_clusters.csv
- PLS_loadings.csv

## Data availability

Raw sequencing data are available at NCBI Sequence Read Archive:

PRJNA762012

(Replace with the final accession number.)

## Reproducibility

The repository contains all scripts necessary to reproduce the analyses corresponding to the main figures.
