README
================
Emily
2024-11-14

# Fraser seasonal black carbon

This repository contains the datasets and R markdown file used to
produce figures and tables in the manuscript “Interplay of seasonal
hydrology and landscape topography drives black carbon export in the
Fraser River” by Emily Brown, Sasha Wagner, and Brian P. V. Hunt.

All datasets needed to produce table 1 and figure 2 are included in this
repository. The dataset “Brown_fraserseasonalblackcarbon_data.csv”
contains original research data, which can be accessed from zenodo at the doi
10.5281/zenodo.14172042.

The dataset “hopedischarge_loadestflux.csv” contains river discharge
data for the Fraser River at Hope, which is open source from Environment
and Climate Change Canada, and can be accessed from
<https://wateroffice.ec.gc.ca/index_e.html> (Station ID = 08MF005). This
dataset also includes flux estimates of DOC, DBC, and PBC, which were
calculated using river discharge data and concentration data from
“Brown_fraserseasonalblackcarbon_data.csv” in the program LOADEST.

Snow water equivalent (SWE) data (“SW_DailyArchive.csv”, “SWDaily.csv”)
is open source from the British Columbia Ministry of Environment, and
can be accessed from
<https://catalogue.data.gov.bc.ca/dataset/current-season-automated-snow-weather-station-data>
and
<https://catalogue.data.gov.bc.ca/dataset/archive-automated-snow-weather-station-data>.
The dataset “SNW_ASWS_BC08MF0001watershed.csv” lists the snow weather
station id’s of the stations which are within the watershed of the
Fraser River at Hope, and is a subset of this open source dataset:
<https://catalogue.data.gov.bc.ca/dataset/automated-snow-weather-station-locations>.

Burned area data (“fire_perimeters_2023.csv”,
“fire_perimeters_2024.csv”) is open source from the British Columbia
Wildfire Service, and can be accessed from
<https://catalogue.data.gov.bc.ca/dataset/bc-wildfire-fire-perimeters-historical>
and
<https://catalogue.data.gov.bc.ca/dataset/bc-wildfire-fire-perimeters-current>.

To reproduce the figures and tables in this manuscript, clone this
repository and use the R markdown file “figures_and_tables.Rmd”.

``` r
sessioninfo::session_info()
```

    ## ─ Session info ───────────────────────────────────────────────────────────────
    ##  setting  value
    ##  version  R version 4.3.1 (2023-06-16 ucrt)
    ##  os       Windows 11 x64 (build 22631)
    ##  system   x86_64, mingw32
    ##  ui       RTerm
    ##  language (EN)
    ##  collate  English_Canada.utf8
    ##  ctype    English_Canada.utf8
    ##  tz       America/Vancouver
    ##  date     2024-11-14
    ##  pandoc   3.2 @ C:/Program Files/RStudio/resources/app/bin/quarto/bin/tools/ (via rmarkdown)
    ## 
    ## ─ Packages ───────────────────────────────────────────────────────────────────
    ##  package     * version date (UTC) lib source
    ##  cli           3.6.1   2023-03-23 [1] CRAN (R 4.3.1)
    ##  digest        0.6.33  2023-07-07 [1] CRAN (R 4.3.1)
    ##  evaluate      0.21    2023-05-05 [1] CRAN (R 4.3.1)
    ##  fastmap       1.1.1   2023-02-24 [1] CRAN (R 4.3.1)
    ##  htmltools     0.5.6   2023-08-10 [1] CRAN (R 4.3.1)
    ##  knitr         1.43    2023-05-25 [1] CRAN (R 4.3.1)
    ##  rlang         1.1.2   2023-11-04 [1] CRAN (R 4.3.2)
    ##  rmarkdown     2.24    2023-08-14 [1] CRAN (R 4.3.1)
    ##  rstudioapi    0.15.0  2023-07-07 [1] CRAN (R 4.3.1)
    ##  sessioninfo   1.2.2   2021-12-06 [1] CRAN (R 4.3.3)
    ##  xfun          0.40    2023-08-09 [1] CRAN (R 4.3.1)
    ##  yaml          2.3.7   2023-01-23 [1] CRAN (R 4.3.0)
    ## 
    ##  [1] C:/Users/emmie/AppData/Local/R/win-library/4.3
    ##  [2] C:/Program Files/R/R-4.3.1/library
    ## 
    ## ──────────────────────────────────────────────────────────────────────────────
