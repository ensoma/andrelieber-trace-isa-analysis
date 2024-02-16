FROM mambaorg/micromamba:1.5.1

RUN \
    micromamba create \
        -y -n andrelieber-trace-isa-analysis -c conda-forge -c bioconda \
        quarto==1.3.427 \
        r-base==4.3.2 \
        r-tidyverse==2.0.0 \
        r-patchwork==1.2.0 \
        r-randomcolor==1.1.0.1 \
        r-ggally==2.2.0 \
        r-ggseqlogo==0.2 \
        bioconductor-biostrings==2.70.1 \
        bioconductor-karyoploter==1.28.0  && \
    micromamba clean -y --all

ENV PATH /opt/conda/envs/andrelieber-trace-isa-analysis/bin:$PATH