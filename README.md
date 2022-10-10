# Supplemental Materials: Random Forest Climatic Modeling of Agricultural Insurance Loss Across the Inland Pacific Northwest Region of the United States

Submitted to Environmental Data Science 2022

Erich Seamon, Paul E. Gessler, John T. Abatzoglou, Philip W. Mote, Stephen S. Lee

April 2022

## Overview:

The following analyses examine agricultural commodity loss, at a county level, from 2001-2015, across the 24 county region of the Inland Pacific Northwest (IPNW). In this analysis, we use a time lagged matrix approach to examine a range of combinations of climate and insurance loss for wheat due to drought.

## Data Access Summary:

Data provided include climate correlations, climate matrices, climatological data taken from Abatzoglou's (2013) GRIDMET daily downscaled climate data, as well as wheat commodity pricing data at a county level.

User should only need to download the attached zip file, decompress, and then run the Rmd from the location of data download.  The Rmd contains code to expand any zip files, and load data needed to re-generate the Rmd output (which is included as an html file).

## Description of the Data and file structure:

All data is found within the /data folder. 

seamon_dissertation_dataload.R. This file loads all data dynamically from github into R. This script is run automatically within each appendix Rmarkdown (located in the appendices folder)

/RMA_Rda: RDA database files that contain aggregated PNW insurance loss claim data.

/RMA_csv: Individual CSV insurance claim data files by year.

/RMA_originaldata: Original .txt files for insurance loss claims, by year, for the entire United States. These files are used in Appendix A and Appendix B.

/climate_correlation_summaries. Climate correlation summary data, loaded in Appendix C for modeling.

/climate_matrices. Climate correlation matrices between individual climate variables and wheat/drought insurance loss. Used in Appendix C.

/climate_outputs. Climate pyramid values by county.  Each .csv is in the following format:

 - <climate variable>_<month><months preceding>_<loss_value>_climatecorrelation.csv
 climate variable acroyms:
   - tmmx = maximum temperature
   - fm100 = 100 hour fuel moisture
   - pdsi = palmer drought severity index
   - pet = potential evapotranspiration
   - pr = precipitation
  
 Example: tmmx_jan1_cube_root_loss_climatecorrelations.csv
  
/climatology. Base climatology for the iPNW.

- Contains .csv files that represent climatological mean values, at a monthly, county level, for all years from 1989 to 2015.  Each file is structured in the following format:

  - <state>_<year>_ipnw_summary.  Example: Idaho_1989_ipnw_summary

/counties. County shapefiles.

- UScounties.zip. Zip file which expands into a shapefile of US counties.
- UScounties_conus.zip. Zip file which expands into a shapefile of coterminous US counties 
- counties_fips.csv.  Zip file which expands into a shapefile of US counties, with fips.
- threestate_palouse.zip.  Zip file which expands into a shapefile of the inland Pacific Northwest palouse agricultural counties.
- threestate_southernID.zip.  Zip file which expands into a shapefile of the southern Idaho agricultural region counties.
- threestate_willamette.zip.  Zip file which expands into a shapefile of the willamette valley agricultural region counties.

/states. State shapefiles.

- Contains two files:
  
  - states_conus.zip.  .Zip file which expands into state boundary shapefile.
  - threestate_boundary.zip. .Zip file which expands into shape file for just the three states of Idaho, Washington, and Idaho.

/wheat_prices. Annual wheat prices.

- Contains two files:
  
  - wheat_prices_1989_2015.csv.  Wheat prices from 1989 to 2015
  - wheat_prices_monthly_1998_2017.csv.  Monthly wheat prices from 1998 to 2015.

/CPI. Consumer pricing indexing data.  

- Contains a .zip file, which expands into CPI.csv.

/wheatproduction. NASS wheat production data, used in Appendix A.

