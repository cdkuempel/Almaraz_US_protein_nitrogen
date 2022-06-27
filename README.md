# Overview
This repository accompanies the publication by Almaraz et al. 2022 The impact of excessive protein consumption on human wastewater nitrogen loading of US waters published in Frontiers in Ecology and the Environment. The full text can be found [here](https://esajournals.onlinelibrary.wiley.com/doi/10.1002/fee.2531).

# Repository structure

## 1. data

There are two main data folders

**raw_data**

This folder has two datasets within the repo and two datasets that are saved from scripts.
- The nitrogen loss by age group data and the United States shapefile are contained within the repo.
- The Census_population.Rmd script creates a shapefile for each state that is saved within the State_tract_files folder.
- The Waterhshed_boundaries.Rmd script downloads the US watershed boundary data, which is saved in this folder.
        
*Note that both the state tract files and watershed boundary files are quite large and are thus ignored and not saved within the github repo (see gitignore)*     
        
**output_data**
- This folder contains cleaned and modified data from the raw_data folder, including population per watershed data and nitrogen estimates.

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

Figures created in the Figures.Rmd script are saved in the figures folder. Further processing was performed to modify the Figure 1 legend in powerpoint. Figures 2 and 3 were not made within the repo and are available upon request to the lead author.

