# Hepatocyte-Dual-Omics

The scripts used to generate the figures and tables for:\
Landgraf et al., under review.
***Widespread Discordance Between mRNA, Protein Abundance, and Functional Output During Metabolic Transition***

The preprint version is available at https://doi.org/10.1101/2025.04.15.649020.

------------------------------------------------------------------------

## Reproduction Instructions

All data required for reproducing our analysis and results is found inside the three `required_files` folders. The corresponding outputs are stored in `output` folders. The scripts can be adapted to analyze similar data.

### Scripts Overview

-   **`Script1`**
    -   Generates `differential_abundance_analysis.csv` with log2 Fold Change and adjusted p-values.
    -   Produces PCA plots.
-   **`Script2`**
    -   Outputs `mapped_data.csv`, which includes 1:1 protein-mRNA mappings with Uniprot symbol, accession number, Ensembl symbol, and Ensembl ID. 
-   **`Script3`**
    -   Main script used to make figures shown in the preprint.
------------------------------------------------------------------------

## Software Versions

-   **Operating System:** macOS 11.6.2 (Big Sur)

-   **R:** v4.4.1

-   **RStudio:** v2023.09.1+494

-   **R Packages**

    biomaRt (2.60.1),\
    dplyr (1.1.4),\
    SummarizedExperiment (1.34.0),\
    ggplot2 (3.5.1),\
    tibble (3.2.1),\
    tidyr (1.3.1),\
    PerformanceAnalytics (2.0.4),\
    MSnbase (2.30.1),\
    reshape2 (1.4.4),\
    limma (3.60.6),\
    UpSetR (1.4.0),\
    ggrepel (0.9.6),\
    plyr (1.8.9),\
    data.table (1.17.0)

-   Other operating systems and versions of R / R-studio are likely compatible but have not been tested. Non-standard hardware is not required.

------------------------------------------------------------------------

## Clone the Repository

To clone this repository locally:

``` bash
git clone https://github.com/kosaku-san/Hepatocyte-Dual-Omics
```

------------------------------------------------------------------------

Demo:
No demo is necessary. The scripts can be directly run with the raw data included inside the `required_files` folders. 

Run time: 
1. Script_1 run time: 5 min; 36 sec 
2. Script_2 run time: 0 min; 6 sec
3. Script_3 run time: 0 min; 57 sec

------------------------------------------------------------------------

## Trouble-shooting

A recursive error (shown below) sometimes occurs when running Script 3. This problem can be fixed by restarting the R-studio session and re-opening the Script_3.Rmd file. 

```
Error: no more error handlers available (recursive errors?); invoking 'abort' restart
Warning: type 29 is unimplemented in 'type2char'
Error in scan(file = file, what = what, sep = sep, quote = quote, dec = dec,  : 
  INTEGER() can only be applied to a 'integer', not a 'unknown type #29'
```

