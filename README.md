# Antibiotics calotriton

Data and code repository of the individual-level metagenomic data of Calotriton asper newts.


## 1. Study design

The samples correspond to 4 individuals prior to antibiotics reception and after.

## 2. Bioinformatic procedures

Data processing to generate annotated metagenome-assembled genomes and genome count tables was conducted using the following Snakemake pipeline: [mg_assembly](https://github.com/3d-omics/mg_assembly). Data analysis procedures source from the outputs of this pipeline.

## 3. Data analysis

Samples were analysed together and the code used can be found in the Rmd files stored in the root directory of this repository, while the bookdown-rendered webbook is available at:

[alberdilab.github.io/antibiotics_calotriton](https://alberdilab.github.io/antibiotics_calotriton)

While the webbook provides a user-friendly overview of the procedures, analyses can be directly reproduced using the Rmd documents. Note that the code chunks that require heavy computation have been tuned off using 'eval=FALSE'. To re-render the webbook, you can use the following code:

```
library(bookdown)
library(htmlwidgets)
library(webshot)

render_book(input = ".", output_format = "bookdown::gitbook", output_dir = "docs")
```
