# Andre Lieber TRACE ISA 2024

This repository houses the downstream analysis of the Mouse TRACE ISA.

## Quickstart

Clone the repository locally.

```
git clone https://github.com/ensoma/andrelieber-trace-isa-analysis.git
```

For ease of reproducibility all software is provided in a Docker container.
After installing Docker the following command can be run to generate the report
and figures.

```
docker compose run --rm trace-isa-analysis
```

## Inputs

The inputs for this analysis consist of two types of outputs from the Ensoma
TRACE ISA Snakemake workflow. These include:

1) The annotated insertion site `TSV` files (data/insertion_sites/*.tsv).
2) `FASTA` files of the sequences surrounding the insertion sites
(data/insertion_site_sequences/*.fasta).

## Outputs

The main output of this analysis is an `HTML` report detailing the analysis
and figures generated. Additionally, high resolution vector images of the
figures in the report are made available (results/*.pdf).

## Software

This analysis is made possible by these and other softwares.

* Docker `25.0.3`
* R `4.3.2`
* rmarkdown `2.25`
* markdown `1.12`
* tidyverse `2.0.0`
* patchwork `1.2.0`
* randomcoloR `1.1.0.1`
* ggseqlogo `0.2`
* Biostrings `2.70.1`
* karyoploteR `1.28.0`
