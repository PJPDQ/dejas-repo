# UNDatathon by DJeANS (DeJAS)

In this event, we have utilized data from various sources to analyze and predict bushfires and their potential impact on endangered species and flaged certain regions which lack fire prevention resources.

### Story Map : https://storymaps.arcgis.com/stories/e038ffe87aa44c01ad2a43ec6eb843bc 
### Arcgis integrated spatial Map : https://undatathon.maps.arcgis.com/apps/mapviewer/index.html?webmap=a406dce68acb4bae9fb6382d44551c5c 
### ShinyApp integrated spatial Map : https://ju-stats.shinyapps.io/FireApp/

#### The project is divided into two distinct parts:

#### (a) Mapping Different Layers of Data:
In this part of the project, the goal was to create maps by overlaying various layers of data onto geographical areas. These data layers include information about fire stations, high-risk bush fire areas, biodiversity data, and endangered species areas map. One specific analysis carried out is calculating the distance between fire stations and the centroid (central point) of high-risk bush fire areas. This distance calculation is optimized to identify regions that are at high risk, where endangered species habitats are present, but there might be a lack of fire prevention resources. Essentially, this part of the project involves visually representing the data layers and using spatial analysis to determine areas of concern where the convergence of high risk and the presence of endangered species meet with a potential lack of fire prevention resources.

#### (b) Predictor:
In the second part of the project, the focus is on prediction. Predictors are created using an Artificial Intelligence (AI) model. The model's training data is gathered from diverse sources as mentioned below. After obtaining the historial dependent variables about climates etc, we got the labeles data from historial records of bush fire. These were integrated using same date and geometry information. 

 
## Our analysis relies on data obtained from the following sources:

### Fire History - Wildfires ( Data is collected for mapping (20--) and modeeling (2020-2023) purpose)
#### Data Source: NPWS Fire History https://datasets.seed.nsw.gov.au/dataset/fire-history-wildfires-and-prescribed-burns-1e8b6 
#### Description: This dataset provides valuable information about the history of wildfires and prescribed burns, offering insights into historical fire occurrences.


### Climate Data (For Modelling purpose from Jan, 2020-Nov, 2023)
#### Data Source: CPC - Climate Prediction Center  https://ftp.cpc.ncep.noaa.gov/cadb_v2/daily/ 
#### Description: daily data obtained from the Climate Prediction Center. This data helps us in forecasting and understanding the dynamics of bushfires. 

### Threatened Species (For Mapping purpose)
#### Data Source: https://www.iucnredlist.org/resources/spatial-data-download
#### Description: The IUCN Red List of Threatened Species™ contains global assessments for more than 150,300 species. More than 82% of these (>123,600 species) have spatial data.
#### Note: So far in our R-shiny App, we only integrated Mammals and Reptiles.

### Fire Station Data (For Mapping purpose)
#### Data Source: Fire and Rescue NSW (FRNSW) https://www.fire.nsw.gov.au/ 
#### Description: This data provide us with the number of fire station in NSW. More details of the extraction https://github.com/PJPDQ/dejas-repo/blob/main/fire_station_fetcher.ipynb 


### Hosting the Open-Sourced R-Shiny App:
As part of our efforts, we have developed an open-source R-Shiny application that integrates geospatial data related to bushfires, fire stations, and endangered species. The primary objective of this application is to highlight regions at high risk of wildfires and are habitat of endangered species.
#### Link for ShinyApp: https://ju-stats.shinyapps.io/FireApp/

### Results

##### Example of critical area (Identified areas) Read more here https://storymaps.arcgis.com/stories/e038ffe87aa44c01ad2a43ec6eb843bc 

##### Layer 1: Bushfire prone and affected areas for the year 2019-2020
 <p align="center">
 <img src="https://github.com/PJPDQ/dejas-repo/assets/45668229/5d5d6abf-9586-45e7-b83c-3e4bf633712a.png"  width="88%" height="400">&nbsp; &nbsp; &nbsp; &nbsp;
</p>

#####  Layer 2 : Existing fire-stations facility in NSW
<p align="center">
<img src="https://github.com/PJPDQ/dejas-repo/assets/45668229/d51ffe1d-1077-41d5-99bc-ce338d69d615.png"  width="88%" height="400">
</p>

#### Layer 3: Identifying the geographic boundaries of state forest regions and the habitats of endangered species in the state of New South Wales.
<p align="center">
<img src="https://github.com/PJPDQ/dejas-repo/assets/45668229/cd4955ae-b340-4582-a911-5fe9f09e73bc.png"  width="88%" height="400">
</p>

#### Layer 4: Optimal coverage area, location and count of the fire-stations
<p align="center">
<img src="https://github.com/PJPDQ/dejas-repo/assets/45668229/cd4955ae-b340-4582-a911-5fe9f09e73bc.png"  width="88%" height="400">
</p>

### Fire stations

<p align="center">
<img src="https://github.com/PJPDQ/dejas-repo/assets/45668229/f9c1ed76-5dea-4ba6-a3b6-53453a419c5e.png"  width="88%" height="400">
</p>

##Future Directions: To advance our research, we envision several promising avenues for future work.

### Enhanced Data Integration: 
Future endeavors should prioritize the incorporation of an even broader range of data sources for training our AI model. This could encompass the integration of satellite-derived vegetation change data over time, soil moisture measurements, and more. Such diverse datasets can significantly improve the model's accuracy and applicability.

### Global Scale Analysis: 
We see potential in expanding our work to a global level analysis. 

### Small-Area Endangered Species Quantification: 
Delving into localized quantification of endangered species can yield valuable insights. Focusing on smaller geographical areas allows for more precise conservation efforts and habitat protection. However, it's crucial to emphasize that such efforts depend heavily on comprehensive surveys and open access to relevant data sources.

In summary, these future directions encompass the integration of diverse data sources, global-scale analysis, and localized quantification of endangered species. The success of these endeavors will be contingent on collaborative survey efforts and the availability of open-access data.

## MIT License

Copyright (c) 2023 Dicky Sentosa, Amarinder Singh Thind, John Uesi, Surekha Gaikwad

Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.

