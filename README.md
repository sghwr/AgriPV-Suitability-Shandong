# AgriPV-Suitability-Shandong

A geospatial analysis project for assessing "PV + Sheep farming" (photovoltaic + pastoralism) development potential in Shandong Province, China. This project uses Spatial Principal Component Analysis (SPCA) to evaluate suitability at 5km×5km grid resolution.

Key Features
Spatial Analysis: 5km×5km grid-based suitability assessment

Methodology: Spatial Principal Component Analysis (SPCA) for multi-factor evaluation

Data Integration: Solar radiation, NDVI, slope, GDP, and existing PV farm data

Visualization: Static (Matplotlib) and interactive (Folium) suitability maps

Data Layers
Solar radiation (interpolated from station data)

NDVI (500m resolution, resampled)

Slope (30m resolution, downsampled)

Urban GDP and influence

Existing PV farm locations

Suitability Index Formula
S = 0.35R_norm + 0.25N_norm + 0.15S_norm + 0.15D_norm + 0.10I_norm

R: Solar radiation (positive)

N: NDVI (optimum at 0.35)

S: Slope (negative)

D: Distance to cities (negative)

I: Urban influence (positive)

Outputs
Suitability classification maps (5 classes from "Unsuitable" to "Highly Suitable")

Validation with existing PV farm locations

Interactive HTML maps for exploration

Tech Stack
Python (Pandas, Geopandas, Rasterio, Matplotlib, Folium, Scikit-learn)

Applications
Supports decision-making for agrivoltaic and PV-pastoralism development in Shandong Province.
