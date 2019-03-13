FROM r-base:3.5.2

# 

# Add R libraries under /tmp
COPY libraries/* /tmp/
# Install R packages
RUN R CMD INSTALL '/tmp/RandomForestExtended.tar.gz'  && \
Rscript -e "install.packages('snow')"
