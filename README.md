# Cows-and-Goats-Microbiome-Data-Analysis
This repository contains the scripts and input data for the biostatistical analysis used in:

Corral-Jara et al.
"Species-specific rumen microbial responses to dietary inhibition of methanogenesis in cows and goats"

Two.Rmd files can be found in the repository: one for cow analysis (statistical_pipeline_cows.Rmd) and the other for goat analysis (Statistical_pipeline_goats.Rmd).

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


=The packages required are:
- DESeq2
- ccrepe
- igraph
- mixOmics
- KEGGREST
- dplyr
- plyr
- data.table

To install all the required packages, please refer to the file Packages_download_data in this repository. 

## Input files

The following input files are required:

Cows:
- BGI_vaches_RNA_seq.csv
- OTUs_vaches.csv
- coldata_vaches.csv
- metabolites.csv
- CH4.csv
- CH4.milk.csv
- CH4.FPCM.csv
- CH4_MSI.csv
- CH4.CO2.csv

Goats:
- BGI_chevres_RNA_seq.csv
- OTUs_chevres.csv
- coldata_chevres.csv
- metabolites_goats.csv
- CH4_goats.csv
- CH4.milk_goats.csv
- CH4.FPCM_goats.csv
- CH4_MSI_goats.csv
- CH4.CO2_goats.csv

## Output files

- deKOs_COS_CTL.csv
- deOTUs_COS_CTL.csv
- network_edges.csv
- kmeans_clusters.csv
- PLS_loadings.csv

The input and output files associated with each figure are described within the corresponding R Markdown (Rmd) files, where the complete workflow for generating each figure is provided.


## Preparation of data and download in RStudio
To prepare and download the data required for the analysis, please refer to the file "Packages_download_data" in this repository. 



