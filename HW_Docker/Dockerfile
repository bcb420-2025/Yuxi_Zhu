# Use the correct arm64-compatible base image
FROM risserlin/bcb420-base-image:winter2025-arm64

# Update and install R libraries
RUN R -e "install.packages(c('BiocManager'), repos='http://cran.us.r-project.org')" && \
    R -e "BiocManager::install(c('DESeq2', 'pheatmap', 'enrichplot'))"

