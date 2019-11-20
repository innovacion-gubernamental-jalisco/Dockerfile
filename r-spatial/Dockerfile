FROM rocker/verse:3.6.0
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
    unixodbc-dev \
  && install2.r --error \
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
    velox\ 
    fasterize\
    spdep \
    geoR \
    tmap \
    geosphere \
    gdalUtils \
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
    ## from bioconductor
    && R -e "BiocManager::install('rhdf5')"  \
    && R -e "devtools::install_github('loicdtx/bfastSpatial')"\
    && R -e "devtools::install_github('16EAGLE/getSpatialData')"
