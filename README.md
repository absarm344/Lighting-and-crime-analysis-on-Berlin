# Berlin Urban Analysis: Streetlights & Safety

## Overview
This project performs a geospatial analysis of Berlin, Germany, focusing on the relationship between urban infrastructure (specifically streetlighting) and social indicators (crime rates). By aggregating distinct planning areas (LORs) into larger administrative districts (Bezirksregionen), the analysis aims to visualize infrastructure inequality and correlate it with safety metrics.

## Key Features
* **Geospatial Aggregation:** Merges granular "Lebensweltlich orientierte Räume" (LOR) data into broader "Bezirksregionen" (BZR) for district-level analysis.
* **Infrastructure Metrics:** Calculates streetlight density (lights per km²) for every district in Berlin.
* **Crime Data Integration:** Cleans and aggregates 2023 crime statistics (Total crimes, Robbery, Theft, Bodily Injuries) to match geospatial boundaries.
* **Interactive Visualization:** Generates Folium maps to visualize district boundaries and attributes interactively.
* **Inequality Analysis:** Quantifies the "Infrastructure Gap" by comparing the top 10% best-lit districts against the bottom 10%.

## Data Sources
The project relies on three primary datasets:
1. **`berlin_lor.geojson`**: Geospatial polygon data for Berlin's planning areas.
2. **`Berlin_streetlights.geojson`**: Point data representing individual streetlight locations.
3. **`Crime_data_2023.csv`**: Statistical data containing crime counts indexed by Region ID.

## Prerequisites
To run this notebook, you need Python installed with the following libraries:

```bash
pip install pandas geopandas folium matplotlib seaborn numpy