# Citi Bike Ridership Data Spatial Join

This Jupyter Notebook file contains the functions necessary to perform a spatial join on Citi Bike's [openly published ride data](https://citibikenyc.com/system-data) by corresponding each Citi Bike station to the official __NYC Tabulation Area__ where it is located.

The functions outlined in the [bikeshare](bikeshare.ipynb) will help you group Citi Bike rides by start/end neighborhoods, with one example being __grouping rides starting/ending in the newly introduced congestion pricing area,__ or in a particular borough, cluster of neighborhoods, etc.

Please do not remove files beginning with `nta2020` as they are the necessary shapefiles to peform the spatial join.
