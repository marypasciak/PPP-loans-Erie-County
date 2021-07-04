#### PPP-loans-Erie-County

PPP loan data downloaded from https://data.sba.gov/dataset/ppp-foia
NAICS data from https://gist.githubusercontent.com/kinlane/8ac0f808fe5f2e16be5b4273ed8d8667/raw/368ea0e1e2c6df3da7b693fd9f14e32320dc6daa/naics-codes.csv

Code at https://github.com/marypasciak/PPP-loans-Erie-County/blob/main/PPP-loans-Erie-County.ipynb

From the SBA site, three .csv files containing PPP loan data were imported. All three have the same data structure. The three files were concatenated into a single file containing 2,770,387 rows.

Data were filtered first for New York State, then for Erie County.

The relevant columns were extracted.

This pared down Erie County data were grouped by NAICS code and aggregated by total number of loans, total number of jobs, sum of loan amount, and sum of forgiveness amount. A new csv was created.

The NAICS code data were read in. The data type of the NAICS_code column was converted to float so that it would match the corresponding NAICSCode column in the Erie County .csv.

The two files were merged using the NAICS codes. This merged file was used for the data analysis.

Two data visualizations were created: https://docs.google.com/document/d/1dlI1BhvwKgX1GJi7Pi5Py3D889XNTgI-noZaE8pcjeQ/edit?usp=sharing
