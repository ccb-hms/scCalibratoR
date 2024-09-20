# scCalibratoR

**scCalibratoR** is a Bioconductor package designed to streamline the process of aligning single-cell RNA sequencing (scRNA-seq) datasets from different batches or sources. It also provides tools for identifying and correcting potential misannotations in cell populations by highlighting the genes responsible for discrepancies.

## Features

- **Batch Effect Correction**: Align single-cell datasets to a trusted reference dataset, mitigating technical noise while preserving biological signals.
- **Annotation Refinement**: Detect and correct potentially misannotated cells by comparing gene expression profiles to reference profiles.
- **Gene Driver Identification**: Identify specific genes driving annotation discrepancies, facilitating targeted corrections.
- **Visualization and Reporting**: Generate visualizations and reports to summarize alignment and correction processes, aiding in interpretation and validation.

# Installation

To install the development version of the package from GitHub use the following command:

``` r
BiocManager::install("ccb-hms/scCalibratoR")
```

NOTE: you will need the [**BiocManager**](https://cran.r-project.org/web/packages/BiocManager/index.html) package to install from Bioconductor.

To build the package vignettes upon installation use:

``` r
BiocManager::install("ccb-hms/scCalibratoR",
                     build_vignettes = TRUE,
                     dependencies = TRUE)
```
