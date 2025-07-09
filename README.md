# Citibike Ridership Data Neighborhood Identifier

This is a Pandas script that corresponds the start/end coordinates of Citibike rides with NYC neighborhoods.

### Why?

Lyft, the owner of Citibike, publishes anonymous ridership data at the start of every month. These datasets contain the information about where and when the rides start, how they end, and whether the rider held a Citibike subscription. While the data is used in Lyft's own reports, it is also [available](https://citibikenyc.com/system-data) for the public.

One thing Lyft __does not__ do is identify which neighborhoods correspond to the start/end coordinates. I was working on a data story about the effects of congestion pricing in NYC and got very disappointed by that.

### How?

I used the official shapefile for the [2020 NYC Tabulation Areas](https://data.cityofnewyork.us/City-Government/2020-Neighborhood-Tabulation-Areas-NTAs-/9nt8-h7nd/about_data) and Nominatim to correspond each pair of coordinates with the neighborhood to which they belong. I created two additional columns (`start_neighborhood` and `end_neighborhood`) so the data would be easier to work with.

I was specifically working with the March 2024 and March 2025 datasets, which you don't have to do. Just go to the Lyft website and look up the name of the file you wish to import. By following the scripts outlined [here](bikeshare.ipynb), you can learn to perform a spatial join from start to finish for your own projects.

### Use, sharing, contributing

Feel free to use this code however you want. Perhaps in the future I can turn this into a library of useful Pandas scripts for data journalists.

### Notes

1. Please do not remove or modify the `shapefiles` folder.
2. This notebook contains functions specific to my project (I was researching the rides between Brooklyn and Manhattan, specifically the congestion relief zone). Feel free to remove them before running the script on your machine.
