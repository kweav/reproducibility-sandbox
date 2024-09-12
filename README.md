# README

# Acute Myeloid Leukemia Heatmap Analysis

This repository contains R code for analyzing and visualizing RNA-seq data from acute myeloid leukemia (AML) samples. The analysis uses data from Shih et al., 2017 [1] and was adapted from the refine.bio examples [3].

## Purpose

This analysis aims to:

1. Load and preprocess RNA-seq data from AML model mice
2. Perform clustering and dimensionality reduction on the data
3. Generate heatmaps to visualize sample and gene relationships
4. Annotate the heatmaps with sample metadata

## Data Source

The RNA-seq data used in this analysis comes from Shih et al., 2017 [1]. Specifically:

- Dataset: SRP070849
- Source: refine.bio [3]
- Number of samples: 19
- Sample type: AML model mice
- Treatment conditions: Vehicle vs. AG-221 (IDH2 mutant) and Vehicle vs. 5-Azacytidine (TET2 mutant)

## Setup

To run this analysis, follow these steps:

1. Clone this repository
2. Ensure you have R and RStudio installed
3. Install required packages (see below)

## Required Libraries

- pheatmap
- magrittr
- dplyr
- readr
- tibble
- sessioninfo

Install these packages using:

`r install.packages(c("pheatmap", "magrittr", "dplyr", "readr", "tibble", "sessioninfo"), dependencies = TRUE)`


## Usage

To run the entire analysis, execute the R script in the root directory. This will generate several outputs:

1. Plots in the `plots` directory
2. Results in the `results` directory

## Outputs

- `aml_heatmap.png`: Annotated heatmap showing sample and gene clustering
- `top_90_var_genes.tsv`: Top 90 genes by variance
- Various intermediate results in the `results` directory

## References

[1] Shih, A. H., et al. (2017). Mutant IDH drives solid tumors to acquire features of glioblastoma stem cells. Cancer Cell, 32(2), 227-242.e8. https://doi.org/10.1016/j.ccell.2017.07.005

[2] Adapted from: https://alexslemonade.github.io/refinebio-examples/03-rnaseq/clustering_rnaseq_01_heatmap.html

[3] https://www.refine.bio/

## Contact

For questions or contributions, please add issues or a PR to the repository.

