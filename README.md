# Brockington_FinalProject

## Summary

This repository was created as part of the final project for Environmental Data Analytics. This project is focused on bat activity along the Colorado River in Grand Canyon, AZ. The repository contains raw data files, processed data files, raw code for processing, wrangling, and analyzing data, and the final knitted report. This study seeks to explore the relationship between bat activity and various environmental variables, through linear models and time series analyses. The data used in this study was originally collected between 2017-2020, however this study was conducted in April, 2023.


## Investigators

Laura Brockington, Duke University, laura.a.brockington@duke.edu, graduate student


## Keywords

Bat survey, acoustic survey, insect sampling, Colorado River, Grand Canyon, discharge


## Database Information

Bat activity dataset (USGS):
Link: https://www.usgs.gov/data/bat-activity-and-insect-abundance-data-along-colorado-river-grand-canyon-az
Accessed Mar 30, 2023

Discharge dataset (USGS):
Link: https://waterdata.usgs.gov/nwis/dv
Accessed Mar 30, 2023


## Folder structure, file formats, and naming conventions 

Folder Code:
- File Data_Analysis.Rmd: R markdown file of data wrangling and analysis
- File Data_Processing.Rmd: R markdown file of data processing and exploration
Folder Data:
- Folder Processed:
	- File Bat_Activity_Insect_Abundance_Data_Processed.csv: CSV file of processed bat activity data
	- File daily_discharge_processed.csv: CSV file of processed discharge data
- Folder Raw:
	-Folder az_hydro_routesNAD83: shape file of rivers in Arizona
	- File Bat_Activity_Insect_Abundance_Data.csv: CSV file of raw data from USGS on bat activity
	- File rawDailyData_COriver_discharge.csv: CSV file of raw data from USGS on discharge in Colorado River
Folder Output:
- File Brockington_ENV872_Project.html: final knitted html report
File README: text file containing metadata related to the project and its data
File Brockington_FinalProject.Rproj: R project file 


## Metadata

Bat activity dataset:

| Variable         | Description                                                      | Class | Units ||:-----------------|:-----------------------------------------------------------------|:------|:------|| Date             | Date of survey                                                   | Date  | N/A   || Daily Temp       | Average temperature on date of survey                            | Num   | °C    || Tall Veg         | Tall vegetation cover as a proportion of the total riparian area | Num   | Ratio || Total Calls      | Total number of recorded bat calls                               | Int   | Count || Total Prey Rate  | Total number of insects collected over the duration of sampling  | Num   | Ratio |


Discharge dataset:

| Variable  | Description                             | Class | Units   |
|:----------|:----------------------------------------|:------|---------|
| Date      | Date of data collection                 | Date  | N/A     |
| Discharge | Volume of water flowing through channel | Num   | ft³/sec |


## Scripts and code

Two codes files (Data_Analysis.Rmd and Data_Processing.Rmd are contained in the Code folder to provide a replicable model for how this study was conducted and where the results came from.


## Quality assurance/quality control

Longitude and latitude coordinates were mapped in ensure quality control.
