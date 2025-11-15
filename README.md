# KMC_FLood_Mapping
Flood Mapping of Kathmandu Metropolitan City
Flood Mapping Using Sentinel-1 SAR in Google Earth Engine

This project uses Sentinel-1 SAR imagery to detect and map flooded areas before and after a flood event. The workflow includes preprocessing, change detection, noise removal, and basic damage assessment for cropland, urban areas, and population.

Features

Imports AOI from a user asset.

Filters Sentinel-1 VH images (descending orbit).

Creates before/after mosaics and applies speckle filtering.

Performs flood detection using SAR ratio thresholding.

Removes permanent water and noisy pixels.

Masks slopes >5° using HydroSHEDS DEM.

Calculates:

Flooded area

Affected cropland (MODIS LC)

Affected urban area

Exposed population (GHSL)

Datasets

Sentinel-1 GRD (SAR)

JRC Global Surface Water (seasonality)

MODIS MCD12Q1 (land cover)

GHSL Population Density

HydroSHEDS DEM

Outputs

Flood extent raster and vector

Exposed population map

Affected cropland and urban area layers

How to Use

Open Google Earth Engine Code Editor.

Paste the .js script into a new file.

Replace the AOI asset with your own if needed.

Modify flood dates and run the script.

Export results to Google Drive.
