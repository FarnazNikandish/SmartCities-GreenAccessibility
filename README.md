# Green Accessibility Analysis – Toronto

This project examines neighbourhood-level access to public green spaces in Toronto using GIS-based spatial analysis. The goal is to quantify variations in green accessibility, identify areas with lower access, and visualize spatial patterns that may be relevant for urban planning and policy discussions.

## Objectives
- Measure green space accessibility across Toronto neighbourhoods  
- Identify neighbourhoods with relatively low access to public greenspaces  
- Explore spatial differences using GIS-based indicators and maps  

## Data Sources
- Toronto Neighbourhood Boundaries (GeoJSON)  
- Toronto Public Greenspaces (GeoJSON)  

## Methodology
The analysis is conducted using GeoPandas and includes the following steps:

- Coordinate reference system (CRS) transformation to a metric projection for accurate distance and area calculations  
- Calculation of neighbourhood areas and total green space area within each neighbourhood using spatial joins  
- Distance-based accessibility analysis using neighbourhood centroids and nearest green space distance  
- Construction of a Green Access Index (GAI), combining green space area ratio and distance to the nearest green space  
- Buffer-based analysis using a 300-meter green space buffer to calculate Green Buffer Coverage (GBC_300), defined as the percentage of each neighbourhood located within walkable distance of greenspaces  
- Visualization of results using choropleth maps  

## Results
The results show notable variation in green space accessibility across Toronto neighbourhoods. Several neighbourhoods exhibit relatively low Green Access Index values and low buffer coverage, suggesting potential gaps in walkable access to greenspaces. These areas may represent priority zones for further investigation or planning-focused interventions.

## Outputs
- Neighbourhood-level accessibility indicators (GAI and GBC_300)  
- Choropleth maps illustrating spatial patterns of green accessibility  

## Tools
- Python  
- GeoPandas  
- Pandas  
- Matplotlib  
- Jupyter Notebook  

## Future Work
Potential extensions of this analysis include:
- Expanding the buffer analysis to additional distances (e.g., 500m, 800m)  
- Integrating socio-economic or demographic data  
- Applying spatial statistical methods to further examine accessibility patterns  


