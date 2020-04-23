FROM rocker/verse:3.6.3
MAINTAINER "Carl Boettiger" cboettig@ropensci.org

RUN apt-get update \
  && apt-get install -y --no-install-recommends \
    lbzip2 \
    libfftw3-dev \
    libgdal-dev \
    libgeos-dev \
    libgsl0-dev \
    libgl1-mesa-dev \
    libglu1-mesa-dev \
    libhdf4-alt-dev \
    libhdf5-dev \
    libjq-dev \
    liblwgeom-dev \
    libpq-dev \
    libproj-dev \
    libprotobuf-dev \
    libnetcdf-dev \
    libsqlite3-dev \
    libssl-dev \
    libudunits2-dev \
    netcdf-bin \
    postgis \
    protobuf-compiler \
    sqlite3 \
    tk-dev \
    unixodbc-dev

RUN install2.r --error \
    shinyjs \
    rmapshaper \
    RColorBrewer \
    RandomFields \
    RNetCDF \
    classInt \
    deldir \
    gstat \
    hdf5r \
    lidR \
    mapdata \
    maptools \
    mapview \
    mapedit \
    ncdf4 \
    proj4 \
    raster \
    rasterVis \
    rgdal \
    rgeos \
    rlas \
    devtools\
    sf \
    sp \
    spacetime \
    spatstat \
    #velox\ 
    fasterize\
    spdep \
    geoR \
    tmap \
    geosphere \
    gdalUtils \
    googleComputeEngineR \
    googledrive \ 
    googleCloudStorageR \
    googleAuthR  \
    RStoolbox \
    remote \
    lubridate \
    snow \
    zoo \
    h2o \
    np \
    tsibble \ 
    reshape2 \
    ROCR \
    corrplot \
    ranger \
    ## from bioconductor
    && R -e "BiocManager::install('rhdf5', update=FALSE, ask=FALSE)"\
    && R -e "devtools::install_github('loicdtx/bfastSpatial')"\
    && R -e "devtools::install_github('16EAGLE/getSpatialData')"
