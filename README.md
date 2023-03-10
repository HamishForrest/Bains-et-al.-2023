# Bains-et-al.-2023
Supplementary data and analysis for "Comprehensive longitudinal study of home-cage activity, including climbing, reveals new complex phenotypic profile in the N171-82Q HD mouse model with implications for refined preclinical studies."

## Purpose
This repository houses data, code and example analysis outputs to align with Frontiers guidelines to authors. 

## Use
### /data
This folder contains data to be analysed by R scripts. 
* **cage_sum_60hr_last_30_mean_HD.csv**
     
     Data summed within a cage and averaged over the last 30 minutes of darkness per day of recording. Three days of recording in total. 

* **cage_sum_60hr_first_30_mean_HD.csv**
     
     Data summed within a cage and averaged over the first 30 minutes of darkness per day of recording. Three days of recording in total. 

* **cage_sum_60hr_period_mean_C57BL6J.csv**
     
     Data summed within a cage and averaged over light and dark periods per day of recording. Three days of recording in total.

### /analysis code
This folder contains R scripts to analyse data using lmer package. 

* **C57BL6J_distance&climbing_dark&light_periods_Rscript.txt**
     
     R script to run over cage_sum_60hr_period_mean_C57BL6J.csv. Please update file names (line 10), Distance/Climbing (line 11) and Light/Dark (line 12) as required. 
     
* **HD_distance&climbing_first30_RScript.txt**
     
     R script to run over cage_sum_60hr_first_30_mean_HD.csv. Please update file names (line 10) and Distance/Climbing (line 11) as required. 

* **HD_distance&climbing_last30_RScript.txt**
     
     R script to run over cage_sum_60hr_last_30_mean_HD.csv. Please update file names (line 10) and Distance/Climbing (line 11) as required. 
     
### /analysis output
This folder contains output files from /analysis code which are used to generate p values for the publication and figures. 

Below is a table indicating which output files, scripts and datasets correspond to one another. 

| analysis output | analysis code | data| 
| --- | --- | --- |
|emm_cage_sum_60_hr_C57BL6J_Dark_distance.csv emm_cage_sum_60_hr_C57BL6J_Dark_climbing.csv emm_cage_sum_60_hr_C57BL6J_Light_distance.csv emm_cage_sum_60_hr_C57BL6J_Light_climbing.csv|C57BL6J_distance&climbing_dark&light_periods_Rscript.txt|cage_sum_60hr_period_mean_C57BL6J.csv|
|emm_cage_sum_60_hr_last_30_HD_distance.csv emm_cage_sum_60_hr_last_30_HD_climbing.csv|HD_distance&climbing_last30_RScript.txt|cage_sum_60hr_last_30_mean_HD.csv|
|emm_cage_sum_60_hr_first_30_HD_distance.csv emm_cage_sum_60_hr_first_30_HD_climbing.csv|HD_distance&climbing_first30_RScript.txt|cage_sum_60hr_first_30_mean_HD.csv|
