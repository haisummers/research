# Environmental Burden of Indoor Cannabis Production

This repository contains code to replicate the analysis from: “Green isn’t Green: The Environmental Burden of Indoor Cannabis Production.” 

# Requirements

This code was developed in Matlab R2017a and will require this version or newer to run. Outputs are written in an .xlsx format and will need Microsoft Excel to open.

•	Basic Replication

File Extraction and Set Up: These instructions will generate results for the 1,011 locations analyzed in the analysis (results of Supplemental Table 11). Download the "Indoor Cannabis Analysis.zip" and extract all files to one folder. Within this folder where the files now reside, create a new folder titled "TMY3."  From my other GitHub respository, titled "TMY3" found here https://github.com/haisummers/TMY3, download all 1,011 files as a .zip. Extract all 1,011 "TMY3-master.zip" files into the folder you created titled "TMY3" that lives inside the folder where your "Indoor Cannabis Analysis.zip " files were extracted. At the end, you should have a root folder with the files from "Indoor Cannabis Analysis.zip" (the files listed below in the supporting files section) and a folder among this files titled "TMY3." Inside the "TMY3" folder should be 1,011 .csv files.

Open the “indoor_cannabis_all_locations.m” file through Matlab and run. As is, this file will run all 1,011 locations and print results to an Excel File titled "Outputs.xlsx." The "Outputs.xlsx" file will be generated in the root folder where the "indoor_cannabis_all_locations.m" is located. Printed in the file are TMY3 file name, city name, state, greenhouse gas emissions (kg CO2-eq/kg- dried flower), electricity (kWh/kg-dried flower), and natural gas required (MJ/kg-dried flower) for all locations. "ResultsFromManuscript.xlsx" is provided for reference, these are the results generated from the original analysis for all locations.

•	Supporting Files

1) Indoor_Model_Facility_LCAv5 - Matlab function that is the indoor cannabis growth model, performs all material and energy inventory calculations, runs for each location, more info in the commented header of this file
2) Indoor Cannabis Model.xlsx - primary data file that Matlab reads from for input variables
3) Psychrometrics.m - Matlab function that returns any property from a psychrometric chart, required two variables to fix state and a pressure
4) Zipcodes.xlsx - Zipcode, latitude and longitude matched locations that is a database of electricty grid emissions GHGs/kWh 
5) electricityLCIegrid26regionstotal.m - electricity grid emissions matched based on Zipcodes.xlsx and latitude and longitude of TMY3





