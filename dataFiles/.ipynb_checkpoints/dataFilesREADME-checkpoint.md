# Data Files ReadMe

# Notes:
Hospital Pricing Sheets will be in the rawHospitalChargeData folder and named with the provider id as appropriate. 

CMS files will all begin with cms and a description of the file. Include the links in this ReadMe. 

# Cleaned Files
## _"compiledMasterchargesNycHospitals.csv"_
This file was compiled from the downloaded raw files in the _rawHospitalChargeData folder_. column names form the various raw files were aggregated and standardized where appropriate. The providerId column was added to each file to help identify where the dataset originated from. 

The standardized columns in this file that will be used for futher analysis are:

'providerId' = hospital id
'drg' = one type of DRG code
'msDrg' = another type of DRG code
'drgDesc' = description of the medical related services for that specific DRG code
'avgCharges' = reported cost of treatment/procedure/ service. For many hospitals in the dataset, it was an average from the 2017 fiscal year. 
'numDischarges' = some hospitals reported on the number of instances/cases/discharges per DRG code

Any other columns found in this file were included because they were found in the raw files from hospitals' mastercharge sheets where there are no DRG codes.