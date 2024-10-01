# Spatial-NDVI-Changes

This repository contains a Jupyter Notebook that analyses Landsat 8 multispectral imagery to study vegetation changes in the Dogon Plateau region of Mali, located in the Sahel, from 2015 to 2023. The primary goal of this analysis is to assess vegetation patterns using Normalized Difference Vegetation Index (NDVI) calculations and evaluate the sensitivity of NDVI to red band weightings.

## Table of Contents

- Introduction
- Dataset
- Notebook Contents
- Conclusions
- Contributing

## Introduction

This project demonstrates the application of geospatial analysis using Python to investigate environmental changes in the Sahel. By leveraging Python libraries such as rasterio, geopandas, and matplotlib, the notebook processes satellite imagery to detect vegetation patterns. It also incorporates hypothesis testing to verify the statistical significance of observed changes.

## Dataset

The dataset consists of Landsat 8 Collection 2 Level-2 Surface Reflectance imagery obtained from EarthExplorer (USGS) for two time periods: October 2015 and October 2023. The analysis focuses on bands related to vegetation monitoring, including Near Infrared (NIR) and Red, which are essential for NDVI calculations. 

**Note:** The input data files are larger than 25MB, which exceeds GitHub's file size limit. Therefore, the dataset is not included in this repository. You can download the data directly from USGS EarthExplorer and follow the instructions in the notebook to run the analysis. Alternatively, feel free to contact me directly if you would like access to the original data files.

## Notebook Contents

The notebook is structured as follows:

1. **Data Loading and Preprocessing:** Importing libraries, loading Landsat 8 datasets and preparing the data for analysis.
2. **Exploratory Data Analysis:** Producing true and false color composites to visualize the geospatial data.
3. **NDVI Calculation:** Defining and applying the NDVI formula to calculate vegetation indices for both 2015 and 2023 datasets.
4. **Statistical Analysis:** Conducting Mann-Whitney U tests to determine the significance of vegetation changes.
5. **Sensitivity Analysis:** Evaluating the effect of modifying the red band weightings on NDVI values.

## Conclusions

The analysis found a statistically significant increase in vegetation from 2015 to 2023, with a 15.58% rise in shrub and grassland extent. Sensitivity studies further revealed that NDVI values are highly responsive to changes in red band weightings, affecting the interpretation of vegetation changes.

## Contributing

Contributions are welcome! If you have suggestions for improvements or additional analyses, feel free to open an issue or submit a pull request.
