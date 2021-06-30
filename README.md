# Almaraz_US_protein_nitrogen
This repository accompanies the publication by Almaraz et al. 2021 The impact of excessive protein consumption on human wastewater nitrogen loading of US waters in Frontiers in Ecology and the Environment.

# Repository structure

## 1. data

There are two main data folders

- raw_data
        This folder has the raw United States Watershed boundary data and the census populuation data downloaded from the Census_population.Rmd script. Note the data is quite large and is thus not saved within the Github repo.
        
        
 - output_data
        This folder contains cleaned and modified data from the raw_data folder, including population per watershed data and nitrogen estimates.

## 2. scripts

There are three scripts that should be executed in sequential order as follows:
 - Census_population.Rmd
        This script gets census data from the American Community Census 5-year data for population by sex and age group, using the tidycensus package. Note that this takes considerable time to run.
        
 - Watershed_boundaries.Rmd
        This script downloads the Watershed Boundary Dataset (HUC8), processes it and saves it as a new file.
        
 - Population_per_watershed.Rmd
         This script combines the watershed data with the state tract census data to determine the population per watershed
         
 - Figures.Rmd
          This script creates Figures 1, S1 and S2

## 4. figures

Figures created in the Figures.Rmd script are saved in the figures folder. Further processing was performed to modify the Figure 1 legend in powerpoint.

