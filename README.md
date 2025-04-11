# tree_envelope_in_bavarian_cities
This repository contains a Jupyter Notebook that analyzes climate envelope data for Bavarian cities by processing raster data and municipal boundaries. The notebook computes pixel-based metrics for multiple tree species across different future time frames, clips the input rasters by city boundaries, and generates individual GeoTIFF files for every city–species–time frame combination. Finally, the output files are bundled into a ZIP archive to facilitate download.

# Requirements
Ensure you have the following Python packages installed:
- numpy
- pandas
- geopandas
- rasterio
- shapely
- matplotlib

You can install these with pip.

# Data requirements 
This notebook expects the following input files in your working directory:
- Shapefile: 'VG250_GEM.shp', downloadable from: https://www.zensus2022.de/DE/Presse/Grafik/shapefile.html
- Raster Files on climate envelopes: TIFF files corresponding to various tree species and time frames, for example:
    'Rotbuche_2011-2040.tif'. These files are available on request from the authors.
- Raster Files on Landuse: 'ugr2018_germany.tif', downloadable from https://doi.org/10.26084/ioerfdz-r10-urbgrn2018

Nevertheless, intermediate results are also stored in .csv Files:
- results.csv describing the share of climate enevelope in the respective city for specific tree species
- landcover_share.csv describring the landcover share for the cities investigated




# License
This project is licensed under the MIT License.
