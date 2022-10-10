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

/climate_outputs. Climate outputs that are used in Appendix C.

/climatology. Base climatology for the iPNW used in Appendix C.

/counties. County shapefiles used in all appendices.

/states. State shapefiles used in all appendices.

/wheat_prices. Annual wheat prices used in Appendix C.

/CPI. Consumer pricing indexing data used in Appendix A.

/wheatproduction. NASS wheat production data, used in Appendix A.

