FROM mambaorg/micromamba:1.5.1

RUN \
    micromamba create \
        -y -n andrelieber-trace-isa-analysis -c conda-forge -c bioconda \
        wget==1.21.4 \
        r-rmarkdown==2.25 \
        r-markdown==1.12 \
        r-base==4.3.2 \
        r-tidyverse==2.0.0 \
        r-patchwork==1.2.0 \
        r-randomcolor==1.1.0.1 \
        r-ggally==2.2.0 \
        r-ggseqlogo==0.2 \
        bioconductor-biostrings==2.70.1 \
        bioconductor-genomicfeatures==1.54.1 \
        bioconductor-genomicranges==1.54.1 \
        bioconductor-rsamtools==2.18.0 \
        bioconductor-karyoploter==1.28.0  && \
    micromamba clean -y --all

USER root
