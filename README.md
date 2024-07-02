# MSE_GenEpi_2024

Lectures and teaching material for the Genetic Epidemiology Elective Module.

This repository contains:

* `01-rnaseq_lecture`
  - A lecture and a couple of practical sessions, with the source and rendered documents.
    The practical sessions will be delivered in a way that will leave space and time for self-learning.
* `02-rbioc_recap`
  - An essential introduction to R and Bioconductor, oriented to the RNA-seq data analysis.
    This document can be consulted anytime for a refresher of the "Intro to R".
* `03-singlecell_rnaseq`
  - Some bonus content on single cell RNA-seq data. We will touch upon this only if the rest of the material 
    has been fully covered - or upon wish from the participants.

For the practical session:

- open the `MSE_GeneticEpidemiology_2024.Rproj` file in RStudio
- open the `01-rnaseq_lecture/transcriptomics_practical.Rmd` or `02-rbioc_recap/intro_to_r_bioc.Rmd` files to follow along the different chunks
- open the `01-rnaseq_lecture/transcriptomics_practical_in_a_glance.Rmd` for a compact version of the practical session

To make sure you're all set for running the code interactively, run this command:

```
## Install the package to handle all Bioc packages and more
install.packages("BiocManager")

## Install Bioconductor's latest version
BiocManager::install()

## Install all packages we will need for all practical parts
BiocManager::install(
  c(
    ## some packages for basic operations
    "knitr",
    "rmarkdown",
    ## the main DE framework we will use
    "DESeq2",
    ## the data package
    "macrophage",
    ## for the enrichment analyses
    "topGO",
    "clusterProfiler",
    ## some interactive shiny apps and packages
    "pcaExplorer",
    "ideal",
    "GeneTonic",
    "iSEE",
    ## some corollary packages required to run all the code
    "tximeta",
    "org.Hs.eg.db",
    "ExploreModelMatrix",
    "apeglm",
    "pheatmap",
    "iSEEu",
    "edgeR"
  )
)
```


