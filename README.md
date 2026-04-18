# KPG_Geochem
Geochem analysis Trim Cane Creek data
Part of PhD Project for Rhiannon Nolan at the University of New Mexico
Fall 2023-Spring 2028

Folders:
Orig_Data = contains data from published sources as downloaded
Sources for each dataset can be found in the code for 01_Data_Compilation.Rmd and below

Data = CSV files modified from original source to fit format. Some contain added columns (e.g. lat and long added
from source publication or found elsewhere based on locality information in source publication)

Figures = Folder for figures generated using code

R files:
01_Data_Compilation.Rmd
Loads in csv files from data generated in this study and from published sources
Saves test_data, align_data, ref_dat, wk_data .RData objects
test_data = my data as a list of strat sections
align_data = published data as a list of sections
ref_dat = published data as a dataframe
wk_data = my data as a dataframe

02_TimeAlignment.Rmd
Loads .RData files from part 01 and uses dtw to line up sections using d13C and d18O data
Saves biozone_assigned, age_assigned, all_sect .RData objects
biozone_assigned = my data with biozone assigned from dtw analysis from all published sources (mode)
age_assigned = my data with biozone assigned from dtw analysis from Hull data (has absolute ages)
all_sect = my data and published data with biozone specified

03_Data_Plotting.Rmd


04_BiodiversityMetrics.Rmd


References:
