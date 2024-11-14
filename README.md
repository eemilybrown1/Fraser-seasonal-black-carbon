# Fraser seasonal black carbon

This repository contains the datasets and R markdown file used to produce figures and tables in the manuscript "Interplay of seasonal hydrology and landscape topography drives black carbon export in the Fraser River" by Emily Brown, Sasha Wagner, and Brian P. V. Hunt.

All datasets needed to produce table 1 and figure 2 are included in this repository. The dataset "Brown_fraserseasonalblackcarbon_data.csv" contains original research data, which can be accessed from zenodo at ___. 

The dataset "hopedischarge_loadestflux.csv" contains river discharge data for the Fraser River at Hope, which is open source from Environment and Climate Change Canada, and can be accessed from https://wateroffice.ec.gc.ca/index_e.html (Station ID = 08MF005). This dataset also includes flux estimates of DOC, DBC, and PBC, which were calculated using river discharge data and concentration data from "Brown_fraserseasonalblackcarbon_data.csv" in the program LOADEST.  

Snow water equivalent (SWE) data ("SW_DailyArchive.csv", "SWDaily.csv") is open source from the British Columbia Ministry of Environment, and can be accessed from https://catalogue.data.gov.bc.ca/dataset/current-season-automated-snow-weather-station-data and https://catalogue.data.gov.bc.ca/dataset/archive-automated-snow-weather-station-data. The dataset "SNW_ASWS_BC08MF0001watershed.csv" lists the snow weather station id's of the stations which are within the watershed of the Fraser River at Hope, and is a subset of this open source dataset: https://catalogue.data.gov.bc.ca/dataset/automated-snow-weather-station-locations. 

Burned area data ("fire_perimeters_2023.csv", "fire_perimeters_2024.csv") is open source from the British Columbia Wildfire Service, and can be accessed from https://catalogue.data.gov.bc.ca/dataset/bc-wildfire-fire-perimeters-historical and https://catalogue.data.gov.bc.ca/dataset/bc-wildfire-fire-perimeters-current.

To reproduce the figures and tables in this manuscript, clone this repository and use the R markdown file "figures_and_tables.Rmd".
