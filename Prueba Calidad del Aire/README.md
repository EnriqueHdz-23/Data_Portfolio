# Air Quality Analysis – Mexico Public Data

This project explores the use of **public government datasets** to analyze air quality parameters in Mexico. The focus is on retrieving, processing, and visualizing environmental data to evaluate pollution levels and provide insights into air quality trends.

---

## calidadaire_EHG

### Objective
Implementation of a workflow to **collect and analyze air quality data** from Mexico’s public API (SINAICA). The goal is to preprocess environmental parameters, visualize them geographically, and assess temporal trends.

### Libraries Used
- pandas – data manipulation and preprocessing  
- numpy – numerical operations  
- requests – API calls  
- json – parsing API responses  
- datosgobmx client – access to Mexico’s open data API  
- folium – interactive geographic visualization  
- mplleaflet – map rendering with matplotlib integration  

### Dataset
Data retrieved from **SINAICA (Sistema Nacional de Información de la Calidad del Aire)** via the `datosgobmx` client.  
Parameters include pollutant concentrations and metadata such as measurement date and location.  
The dataset is structured in JSON format and converted into pandas DataFrames for analysis.

### Main Results
- Successful connection to the **SINAICA API** and retrieval of valid air quality parameters.  
- Preprocessing included handling JSON responses, concatenating results, and converting timestamps.  
- Interactive maps generated with **folium** and **mplleaflet** to visualize pollutant distribution.  
- Temporal analysis of pollutant levels provided insights into air quality variations across regions.  

---

## Key Takeaways
- Public government APIs provide **valuable and reliable data sources** for environmental analysis.  
- Integration of geospatial libraries (folium, mplleaflet) enables **interactive visualization** of pollution levels.  
- This project demonstrates the ability to combine **data engineering, visualization, and environmental science** for impactful insights relevant to public health and policy.  
