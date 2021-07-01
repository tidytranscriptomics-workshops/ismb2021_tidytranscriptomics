<!-- badges: start -->
[![.github/workflows/basic_checks.yaml](https://github.com/tidy-transcriptomics-workshops/ismb2021_tidytranscriptomics/workflows/.github/workflows/basic_checks.yaml/badge.svg)](https://github.com/tidy-transcriptomics-workshops/ismb2021_tidytranscriptomics/actions) 	
<!-- badges: end -->

# Introduction to Tidy Transcriptomics
<p float="left">
<img height="100" alt="ismb2021" src="https://github.com/Bioconductor/BiocStickers/blob/71e4c2cb323c441daa0f2f9d48d3b8bbb564a3e2/events/ismb2021/ismb2021.png?raw=true"/>
<img height="100" alt="tidybulk" src="https://github.com/Bioconductor/BiocStickers/blob/master/tidybulk/tidybulk.png?raw=true"/>
</p>

## Instructor names and contact information

* Maria Doyle <Maria.Doyle at petermac.org>  
* Stefano Mangiola <mangiola.s at wehi.edu.au>

## Syllabus

Material [web page](https://stemangiola.github.io/ismb2021_tidytranscriptomics/articles/tidytranscriptomics.html).

More details on the workshop are below.

## Workshop package installation 

This is necessary in order to reproduce the code shown in the workshop. The workshop is designed for R `4.1` and can be installed as described below.

```
#install.packages('remotes')

# Need to set this to prevent installation erroring due to even tiny warnings, similar to here: https://github.com/r-lib/remotes/issues/403#issuecomment-748181946
Sys.setenv("R_REMOTES_NO_ERRORS_FROM_WARNINGS" = "true")

# Install workshop package
remotes::install_github("stemangiola/ismb2021_tidytranscriptomics", build_vignettes = TRUE)

# To view vignettes
library(ismb2021tidytranscriptomics)
browseVignettes("ismb2021tidytranscriptomics")
```

To run the code, you could then copy and paste the code from the workshop vignette or [R markdown file](https://raw.githubusercontent.com/stemangiola/ismb2021_tidytranscriptomics/master/vignettes/tidytranscriptomics.Rmd) into a new R Markdown file on your computer.

## Workshop Description

Recently, [plyranges](https://bioconductor.org/packages/release/bioc/html/plyranges.html) and [tidybulk](https://www.bioconductor.org/packages/release/bioc/html/tidybulk.html) have made efforts toward the harmonization of biological data structures and workflows using the concept of data tidiness, to facilitate modularisation. In this workshop, we present [tidySingleCellExperiment](https://stemangiola.github.io/tidySingleCellExperiment/) and [tidySummarizedExperiment](https://stemangiola.github.io/tidySummarizedExperiment/), two R packages that allow the user to visualise and manipulate SingleCellExperiment and SummarizedExperiment objects in a tidy fashion. Importantly, the tidybulk framework now works natively with SummarizedExperiment objects and, thanks to tidySummarizedExperiment, allows tidy and modular RNA sequencing analyses without renouncing the efficiency of Bioconductor data containers. These tools are part of the [tidytranscriptomics](https://github.com/tidy-transcriptomics-workshops/tidytranscriptomics) R software suite, and represent an effort toward the harmonisation of transcriptional analyses under the tidy umbrella.

### Pre-requisites

* Some familiarity with tidyverse syntax
* Some familiarity with bulk RNA-seq and single cell RNA-seq

Recommended Background Reading
[Introduction to R for Biologists](https://melbournebioinformatics.github.io/r-intro-biologists/intro_r_biologists.html)

### Workshop Participation

The workshop format is a 1.5 hour session consisting of hands-on demos and Q&A.

### _R_ / _Bioconductor_ packages used

* tidySummarizedExperiment
* tidySingleCellExperiment
* tidybulk
* tidyHeatmap
* limma
* edgeR
* DESeq2
* airway
* org.Hs.eg.db
* dittoSeq
* ggrepel
* GGally
* plotly


### Time outline

Guide

| Activity - Hands on demos with Q&A                                 | Time |
|--------------------------------------------------------------------|------|
| Part 1 Bulk RNA-seq with tidybulk                                  |  45  |
| Part 2 Single-cell RNA-seq with tidySingleCellExperiment           |  45  |
| Total                                                              |  90m |


#### Learning goals

* To understand how transcriptomic data can be represented and analysed according to the tidy data paradigm with tidySingleCellExperiment and tidySummarizedExperiment.

#### Learning objectives
* Explore and visualise bulk RNA-seq count data with tidySummarizedExperiment
* Explore and visualise single cell RNA-seq  count data with tidySingleCellExperiment
