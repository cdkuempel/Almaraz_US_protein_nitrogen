# Almaraz_US_protein_nitrogen
This repository accompanies the publication by Almaraz et al. 2021 The impact of excessive protein consumption on human wastewater nitrogen loading of US waters in Frontiers in Ecology and the Environment.

# Repository structure

## 1. data

Input data used within the scripts to produce modified data that is saved in the outputs folder. Data used is from Poore and Nemecek 2018 and Hilborn et al. 2018. See the main text and Supplemental materials for further information.

## 2. scripts

There are three scripts that should be executed in sequential order as follows:
 - Census_pop_watershed.Rmd
        This script gets census data
        
 - Watershed_boundaries.Rmd
        This script downloads the Watershed Boundary Dataset (HUC8), processes it and saves it as a new file.
        
 - Population_per_watershed.Rmd
         This script combines the watershed data with the state tract census data to determine the population per watershed
         
 - Figures.Rmd
          This script creates Figures 1, S1 and S2

## 3. outputs

The data created in the theoretical example script are saved in the outputs folder 

## 4. figures

Figures created in the Figures.Rmd script are saved in the figures folder. Further processing was performed to modify the Figure 1 legend in powerpoint.

