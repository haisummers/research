# Environmental Burden of Indoor Cannabis Production

This repository contains code to replicate the analysis from: “Green isn’t Green: The Environmental Burden of Indoor Cannabis Production.” The primary analysis files were generated in Matlab and can be run on versions R2017a or newer.

# Requirements

This code was developed in Matlab R2017a and will require this version or newer to run. Outputs are written in an .xlsx format and will need Microsoft Excel to open.

•	Basic Replication

These instructions will generate results for the 1,011 locations analyzed in the analysis (results of Supplemental Table 11).
Download the "Indoor Cannabis Analysis.zip" and extract all files. Open the “indoor_cannabis_all_locations.m” in Matlab and run. As is, 
the file will run all 1,011 locations and print results to an Excel File title "Outputs.xlsx" that will be generated. The "Outputs.xlsx" file will be generated in the root folder where the "indoor_cannabis_all_locations.m" is located. Printed in the file are TMY3 file name, city name, state, greenhouse gas emissions (kg CO2-eq/kg- dried flower), electricity (kWh/kg-dried flower), and natural gas required (MJ/kg-dried flower) for all locations. "ResultsFromManuscript.xlsx" is provided for reference, these are the results generated from the original analysis for all locations.

•	Supporting Files

1) Indoor_Model_Facility_LCAv5 - Matlab function that is the indoor cannabis growth model, performs all material and energy inventory calculations, runs for each location, more info in the commented header of this file
2) Indoor Cannabis Model.xlsx - primary data file that Matlab reads from for input variables
3) Psychrometrics.m - Matlab function that returns any property from a psychrometric chart, required two variables to fix state and a pressure
4) Zipcodes.xlsx - Zipcode, latitude and longitude matched locations that is a database of electricty grid emissions GHGs/kWh 
5) electricityLCIegrid26regionstotal.m - electricity grid emissions matched based on Zipcodes.xlsx and latitude and longitude of TMY3





