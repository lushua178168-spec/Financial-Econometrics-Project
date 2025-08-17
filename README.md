# Project Overview
This project analyzes the relationship between different types of grant aid — Other Federal Grant Aid, Pell Grant Aid, and State/Local Grant Aid — and graduation rates across U.S. institutions, using 2022–23 IPEDS data and College Scorecard data.

## Files Included
- **Data**
  - `data_sum-v2.xlsx`: Raw data downloaded from IPEDS and College Scorecard.
  - `data_clean.xlsx`: Cleaned dataset, merged using `unitid`, containing all variables used in the project.

- **RMD Files**
  - `dashboard.Rmd`: Flexdashboard source code for interactive visualizations.
  - `The effect of Federal, Pell, State and Local grant aids on Graduation Rates.Rmd`: Report source code.

- **Reports**
  - `The effect ... pdf`: Final report in PDF format.
  - `dashboard link.txt`: Link to the hosted dashboard.

- **Documentation**
  - `README.md`: This instruction file.

## Data Cleaning
Download 2022–2023 semester-year data in IPEDS and College Scorecard. Select useful variables:
`Unitid, Institution name, Year, State, Size, Sector, Degree-granting status, Urban-centric locale, Institutional category, Grad_rate, Ave_fed_grant, Ave_Pell_grant, Ave_state/local_grant, Fed_locale, Pro_pell, pell_grad, loannopell_grad, noloanpell_grad, Net tuition revenue, CITY, ZIP`.

Use VLOOKUP to merge datasets by `unitid`.

## How to Run
1. **Reproduce Flexdashboard**  
   Open `dashboard.Rmd` in RStudio. Ensure `data_clean.xlsx` is in the same folder. Click **Run Document** to generate the dashboard.  

2. **Run R Markdown Report**  
   Open `The effect of Federal, Pell, State and Local grant aids on Graduation Rates.Rmd` in RStudio. Ensure `data_clean.xlsx` is in the same folder. Click **Run Document** to generate the report.
