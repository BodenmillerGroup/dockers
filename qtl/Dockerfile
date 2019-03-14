FROM r-base:3.5.2

# Add R libraries under /tmp
COPY libraries/* /tmp/
# Install R packages
RUN Rscript -e "install.packages('snow')" && \
R CMD INSTALL '/tmp/RandomForestExtended.tar.gz'  && \
R CMD INSTALL '/tmp/RFQTL_diploid_JW.tar.gz' 
