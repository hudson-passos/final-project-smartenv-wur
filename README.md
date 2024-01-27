Background

The learning goals ("Introduction.ipynb") were defined in a way to align some aspects related to data science that I would like to develop during the course, and the technical needs of the group project. Among the criteria also included forming realistic goals to be developed in just three weeks.

Initially, we chose to choose a topic related to air quality, and we would like the study area to be located in Europe, as there is an abundant amount of data and ease of language. In the first researches, we noticed that Poland has very high air pollution levels and this motivated us to seek to better understand the causes and consequences of this case. The project was titled: "Investigating Causes and Impacts of Air Pollution in Poland" and we divided it into three objectives: (1) "Analyze the contribution of sources of Nitrogen Oxides (NOx) to the air pollution in Poland in 2019", (2) "Investigate the relationship between traffic and emissions using machine learning and predict the emission in 2023", and (3) "Investigate the relationship of annual average concentration of PM 2.5 and rate of death caused by respiratory diseases". After the definition of the objectives, we assigned the group members responsible for developing these tasks: the first objective was assigned to Qin Xu (Olive) and I; the second was under Dong Liang; and the third was with Pamungkas Intam and Sabrina Ramadwiriani.

The needs of the first objective were well aligned with what I had defined in my learning goals:

(1) Geospatial analysis in GeoPandas: We did all the geospatial analyses using Pandas and GeoPandas. This learning goal was challenging, especially in terms of generating subplots of multiple GeoPandas objects. However, it was surprising how similar GeoPandas is to Pandas and this made this tool much more familiar than I imagined. Fortunately, all the operations and analyses that I would do with some of the GIS applications, with which I am more familiar, I was able to perform with Pandas/GeoPandas.

(2) Combining information: We were able to combine data from different sources into integrated dataframes. This task was less challenging than the previous one, but more laborious. I still can't make these codes cleaner and more compact. I can do repeated operations with the application of "functions", but I still have difficulty using "classes".

(3) Github: We were able to create our repository on Github and make it our main means of sharing codes. Despite the fact that there are other more specific applications of github that we still do not know (e.g. "version control"), this experience was crucial to introduce us to this resource once and for all. Our Github repository can be found at: https://github.com/hudsonpassos85/DSSE.


Data sources:

- Administrative boundaries: 
  - Source: GIS.Box 
  - Product: boundaries from Poland, voivodeships (provinces), counties and municipalities 
  - Type: shapefile 
  - Spatial distribution: 
  - Link: https://gis-support.pl/baza-wiedzy-2/dane-do-pobrania/granice-administracyjne/
  
- Air pollution: 
  - Source: Inspekcja Ochrony Środowiska 
  - Product: emissions of NOx air pollution (kg) 
  - Type: csv 
  - Spatial distribution: points (air quality measuremente stations) 
  - Link: https://powietrze.gios.gov.pl/pjp/archives 

- Traffic: 
  - Source: Statistics Poland 
  - Product: emissions of NOx air pollution (tonnes) 
  - Type: csv 
  - Spatial distribution: provinces 
  - Link: https://transtat.stat.gov.pl/ 

- Industry: 
  - Source: European Environment Agency  
  - Product: industrial emissions of NOx (kg) 
  - Type: csv 
  - Spatial distribution: points 
  - Link: https://www.eea.europa.eu/en/datahub/datahubitem-view/9405f714-8015-4b5b-a63c-280b82861b3d


The spreadsheet with a detailed description of all the datasets used in the project can be accessed at the link: https://github.com/hudsonpassos85/DSSE/raw/main/Report%20and%20Presentation/Data%20Availability.xlsx





















