# Airbnb in Europe — Exploratory Data Analysis (2023–2024)

Exploratory analysis of Airbnb listings across major European cities using **per-capita metrics**, **quantile-based comparisons**, and **geospatial mapping**.  
The notebook builds interactive visuals (Altair/Seaborn) and Folium/GeoPandas maps, and examines **average income per listing** including a **before/after imputation** comparison.

## Key Questions
- Which cities have the highest Airbnb supply, and how does the picture change **per capita**?
- How do cities compare by **room type**, **licensing status**, **minimum nights**, and **occupancy**?
- What patterns emerge across **neighbourhood × room_type × property_type** price groups?
- How does **income per listing** change **before vs. after** simple imputation of missing values?
- Where are listings concentrated geographically? (interactive city maps)

## Methods & Tools
- **EDA:** pandas, NumPy, groupby aggregations, quantile splits (top/middle/bottom).
- **Visuals:** Seaborn/Matplotlib; **Altair** for interactive charts.
- **Geospatial:** **GeoPandas** for boundaries/joins; **Folium** for interactive maps.
- **Feature Engineering:** per-capita normalization (per 1,000 inhabitants), income per listing; imputation vs. non-imputed comparison.
- **Reproducibility:** parameterized data path, compact helpers, styled tables.

## How to Run
1. Create a Python 3.10+ environment.
2. Install dependencies:
   ```bash
   pip install pandas numpy matplotlib seaborn altair geopandas folium
