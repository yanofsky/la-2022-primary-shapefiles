# Los Angeles County June 7, 2022 Primary Election geodata

This repo contains a geodatabase and geojson files to use with LA County election results from the June 7, 2022 primary.

The files are in the `geojson-by-race` directory.

## Creating the files yourself

To create the files yourself, run the `create-shapefiles.ipynb` Jupyter notebook. It requires Python 3.7, pandas, geopandas, fiona, requests and xlrd. So:

`pip install pandas geopandas fiona requests xlrd`

## Merging election results with the geodata

This repo does not contain the election results. But if you run `create-shapefiles.ipynb` it will download the data and create geojson files that include the election results as properties of each precinct. Those files will be saved into a new folder `geojson-by-race-with-results`

## Where to get LA County election precinct shapefiles

The `DavidYanofsky.gdb` geodatabase was provided to me by the Los Angeles county. You can request your own copy through [their order form](https://survey123.arcgis.com/share/c9c5ad77c3154f699079305adc10aacd). It costs $22 for them to mail a CD to you. And you'll have to mail them a check or go to Norwalk to pay. 

I suggest you just use these files for free.
