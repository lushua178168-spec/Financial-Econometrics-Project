1. Project Overview
This project analyzes the relationship between different types of grant aid — Other Federal Grant Aid, Pell Grant Aid, and State/Local Grant Aid — and graduation rates across U.S. institutions, using 2022–23 IPEDS data and score.

2.Files Included
2.1 data file
2.1.1data_sum-v2.xlsx
The data download from IPEDS and College Scorecard Data. All the sheet and variables have detail descriptions.

2.1.2data_clean.xlsx	
After merging the two original datasets, colleges_cored2022_23_PP and IPEDS_2022_23, using the unique institutional identifier (unitid), we constructed the combined datasets. Cleaned dataset containing all variables used in the project.

2.2RMD file
2.2.1.dashboard.RMD
Flexdashboard source code for interactive dashboard visualizations.

2.2.2.The effect of Federal, Pell, State and Local grant aids on Graduation Rates across U.S institutions.RMD
Pdf report source code.

2.3final report file
2.3.1.dashboard link.txt
The link to final dashboard

2.3.2.The effect of Federal, Pell, State and Local grant aids on Graduation Rates across U.S institutions.pdf
Final report pdf

2.4.readme.docx
This instruction file.

3.Data cleaning
Download 2022-2023 semester year data in IPEDS and colleges_cored.
Select useful variables in IPEDS dataset including Unitid, Institution name, Year, State, Size, Sector, Degree-granting status, Urban-centric locale, Institutional category, Grad_rate, Ave_fed_grant, Ave_Pell_grant, Ave_state/local_grant, Fed_locale, 
Using vlookup to find same uid and fill variables Pro_pell, pell_grad, loannopell_grad, noloanpell_grad, Net tuition revenue, CITY, ZIP. 


4. How to Run
4.1 Reproduce Flexdashboard
Open dashboard.Rmd in RStudio.
Ensure data_clean.xlsx is in the same folder as the Rmd file.
Click run document to generate the dashboard.

4.2 Run R markdown
Open The effect of Federal, Pell, State and Local grant aids on Graduation Rates across U.S institutions.R in RStudio.
Ensure data_clean.xlsx is in the same folder as the Rmd file.
Click run document to generate the dashboard.
