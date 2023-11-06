# UNDatathon by DJeANS (DeJAS)

In this event, we have utilized data from various sources to analyze and predict bushfires and their potential impact on endangered species and flaged certain regions which lack fire prevention resources.

## Our analysis relies on data obtained from the following sources:

### Fire History - Wildfires
#### Data Source: NPWS Fire History https://datasets.seed.nsw.gov.au/dataset/fire-history-wildfires-and-prescribed-burns-1e8b6 
#### Description: This dataset provides valuable information about the history of wildfires and prescribed burns, offering insights into historical fire occurrences.


### Climate Data
#### Data Source: CPC - Climate Prediction Center  https://ftp.cpc.ncep.noaa.gov/cadb_v2/daily/ 
#### Description: daily data obtained from the Climate Prediction Center. This data helps us in forecasting and understanding the dynamics of bushfires. 

### Threatened Species 
#### Data Source: https://www.iucnredlist.org/resources/spatial-data-download
#### Description: The IUCN Red List of Threatened Species™ contains global assessments for more than 150,300 species. More than 82% of these (>123,600 species) have spatial data.
#### Note: So far in our R-shiny App, we only integrated Mammals and Reptiles.

### Fire Station Data
#### Data Source: Fire and Rescue NSW (FRNSW) https://www.fire.nsw.gov.au/ 
#### Description: This data provide us with the number of fire station in NSW. More details of the extraction https://github.com/PJPDQ/dejas-repo/blob/main/fire_station_fetcher.ipynb 


### Hosting the Open-Sourced R-Shiny App:
As part of our efforts, we have developed an open-source R-Shiny application that integrates geospatial data related to bushfires, fire stations, and endangered species. The primary objective of this application is to highlight regions at high risk of wildfires and are habitat of endangered species.


## MIT License

Copyright (c) 2023 [Dicky Sentosa, Amarinder Singh Thind,John Uesi, Surekha Gaikwad]

Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.

