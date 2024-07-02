# MSE_GenEpi_2024

Lectures and teaching material for the Genetic Epidemiology Elective Module.

This repository contains

* `01-rnaseq_lecture`
  - A lecture and a practical session, with the source and rendered documents
* `02-rbioc_recap`
  - An essential introduction to R and Bioconductor, oriented to the RNA-seq data analysis
* `03-interpretation_singlecell`
  - Some bonus content on single cell RNA-seq data

For the practical session, open the `MSE_GeneticEpidemiology.Rproj` file in RStudio, and 
open the `01-rnaseq_lecture/transcriptomics_practical.Rmd` 
or
`02-rbioc_recap/intro_to_r_bioc.Rmd`
files to follow along the different chunks.

To make sure you're all set for running the code interactively, run this command:

```
install.packages("BiocManager")
BiocManager::install()
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


