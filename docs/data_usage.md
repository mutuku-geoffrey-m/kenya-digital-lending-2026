================================================================
DATA USAGE AND SOURCE DOCUMENTATION
Kenya Digital Lending Investment Analysis — February 2026
================================================================

ANALYST
-------
Name:    Geoffrey Mutuku
Project: Investment Due Diligence — Kenyan Digital Lending Sector
Date:    February 2026

================================================================
SECTION 1 — MACROECONOMIC DATA
================================================================

DATASET 1: Commercial Bank Lending Rates
Source:    Central Bank of Kenya (CBK)
Portal:    centralbank.go.ke/statistics/interest-rates
File:      cbk_lending_rate_raw.xlsx
Frequency: Monthly
Range:     2014 to 2025
Units:     Percent (%)
License:   Public — CBK Open Statistics
Use:       Pricing calibration, stress test interest rate driver

----------------------------------------------------------------

DATASET 2: Bank Non-Performing Loans Ratio
Source:    World Bank Open Data
           (CBK direct download unavailable — WB proxy used)
Portal:    data.worldbank.org
Indicator: Bank nonperforming loans to total gross loans (%)
           Code: FB.AST.NPER.ZS
File:      cbk_npl_ratio_raw.xlsx
Frequency: Annual
Range:     2006 to 2023
Units:     Percent (%)
License:   Creative Commons Attribution 4.0
Use:       Probability of default calibration

----------------------------------------------------------------

DATASET 3: Private Sector Credit
Source:    Central Bank of Kenya (CBK)
Portal:    centralbank.go.ke/statistics/monetary-statistics
File:      cbk_private_credit_raw.xlsx
Series:    Claims on Private Sector — Section C
           Depository Corporation Survey (consolidated)
           Covers CBK, Commercial Banks, MFBs and SACCOs
Frequency: Monthly
Range:     2014 to 2025
Units:     KES Millions
License:   Public — CBK Open Statistics
Use:       Market sizing, credit growth driver

----------------------------------------------------------------

DATASET 4: Central Bank Rate (Policy Rate)
Source:    Central Bank of Kenya (CBK)
Portal:    centralbank.go.ke/monetary-policy
File:      cbk_policy_rate_raw.xlsx
Frequency: Per MPC meeting (approximately 6 times per year)
           Forward filled to monthly in cleaning notebook
Range:     2011 to 2026
Units:     Percent (%)
License:   Public — CBK Open Statistics
Use:       Funding cost baseline, stress test rate driver

----------------------------------------------------------------

DATASET 5: Inflation (Consumer Prices)
Source:    World Bank Open Data
           (KNBS direct download unavailable — WB proxy used)
Portal:    data.worldbank.org
Indicator: Inflation, consumer prices (annual %)
           Code: FP.CPI.TOTL.ZG
File:      knbs_inflation_raw.xlsx
Frequency: Annual
Range:     1960 to 2024
Units:     Percent (%)
License:   Creative Commons Attribution 4.0
Use:       Cost pressure driver, real rate calculation

----------------------------------------------------------------

DATASET 6: GDP Growth
Source:    World Bank Open Data
           (KNBS direct download unavailable — WB proxy used)
Portal:    data.worldbank.org
Indicator: GDP growth (annual %)
           Code: NY.GDP.MKTP.KD.ZG
File:      knbs_gdp_raw.xls
Frequency: Annual
Range:     1961 to 2024
Units:     Percent (%)
License:   Creative Commons Attribution 4.0
Use:       Macro stress scenario driver

----------------------------------------------------------------

DATASET 7: Unemployment Rate
Source:    International Labour Organization (ILO)
           Modelled estimates
           (KNBS direct download unavailable — ILO proxy used)
Portal:    ilostat.ilo.org
Indicator: SDG 8.5.2 — Unemployment rate
           Filter: Kenya | Total | Age 15+
File:      knbs_unemployment_raw.xlsx
Frequency: Annual
Range:     2000 to 2024
Units:     Percent (%)
License:   ILO Open Data
Use:       Macro stress driver, PD elasticity calibration

----------------------------------------------------------------

DATASET 8: Population Total
Source:    World Bank Open Data
Portal:    data.worldbank.org
Indicator: Population, total
           Code: SP.POP.TOTL
File:      knbs_population_total_raw.xls
Frequency: Annual
Range:     1960 to 2024
Units:     Persons
License:   Creative Commons Attribution 4.0
Use:       TAM denominator, adult population derivation

----------------------------------------------------------------

DATASET 9: Population Working Age Percent
Source:    World Bank Open Data
Portal:    data.worldbank.org
Indicator: Population ages 15-64 (% of total population)
           Code: SP.POP.1564.TO.ZS
File:      knbs_population_working_age_pct_raw.xls
Frequency: Annual
Range:     1960 to 2024
Units:     Percent of total population
License:   Creative Commons Attribution 4.0
Use:       Adult population derivation for TAM calculation

----------------------------------------------------------------

DATASET 10: Household Income Distribution
Source:    Analyst-constructed from published aggregate sources
           - World Bank Kenya Poverty Assessment 2023
           - KNBS Economic Survey 2024
           - FSD Kenya FinAccess Survey 2021
File:      knbs_income_raw.xlsx
Frequency: Cross-sectional (2021 to 2024 reference period)
Units:     KES Monthly household income
License:   Constructed — sources fully documented in file
Use:       Borrower segmentation, TAM income band breakdown

----------------------------------------------------------------

DATASET 11: GDP Total (Used to derive GDP per capita)
Source:    World Bank Open Data
Portal:    data.worldbank.org
Indicator: GDP (current US$)
           Code: NY.GDP.MKTP.CD
File:      wb_gdp_per_capita_raw.xls
Note:      File contains total GDP not per capita.
           GDP per capita derived in notebook 01 as:
           GDP per capita = Total GDP / Total Population
Frequency: Annual
Range:     1960 to 2024
Units:     USD
License:   Creative Commons Attribution 4.0
Use:       Market context, loan affordability benchmarking

----------------------------------------------------------------

DATASET 12: Domestic Credit to Private Sector % GDP
Source:    World Bank Open Data
Portal:    data.worldbank.org
Indicator: Domestic credit to private sector (% of GDP)
           Code: FS.AST.PRVT.GD.ZS
File:      wb_credit_gdp_raw.xls
Frequency: Annual
Range:     1961 to 2023
Units:     Percent of GDP
License:   Creative Commons Attribution 4.0
Use:       Market opportunity thesis
           Kenya at ~32% vs global average ~90% — gap = TAM

----------------------------------------------------------------

DATASET 13: Interest Rate Spread
Source:    World Bank Open Data
Portal:    data.worldbank.org
Indicator: Interest rate spread
           (lending rate minus deposit rate, %)
           Code: FR.INR.LNDP
File:      wb_interest_spread_raw.xls
Frequency: Annual
Range:     1971 to 2023
Units:     Percentage points
License:   Creative Commons Attribution 4.0
Use:       Pricing analysis, margin compression assessment

================================================================
SECTION 2 — DIGITAL PAYMENTS ECOSYSTEM DATA
================================================================

DATASET 14: M-Pesa Operational Metrics
Source:    Safaricom PLC — Annual Reports and
           Half Year Results Announcements
Portal:    safaricom.co.ke/investor-relations
File:      mpesa_metrics_raw.xlsx
Frequency: Annual / Half year
Range:     2020 to 2024
Units:     Customers (Millions), Transactions (Millions),
           Value (KES Billions)
License:   Publicly disclosed investor relations data
Note:      Manually constructed from PDF reports.
           Source document noted in each row of the file.
Use:       Digital distribution thesis, ecosystem maturity,
           TAM reachability via mobile money

================================================================
SECTION 3 — FINANCIAL ACCESS DATA
================================================================

DATASET 15: IMF Financial Access Survey — Kenya
Source:    International Monetary Fund (IMF)
Portal:    data.imf.org/fas
File:      imf_financial_access_raw.csv
Frequency: Annual
Range:     2004 to 2024
Units:     Various (per 1,000 adults, per 100,000 adults)
License:   IMF Open Data
Use:       Financial inclusion benchmarking,
           mobile money penetration analysis,
           TAM digital reachability calculation

================================================================
SECTION 4 — BORROWER LEVEL DATA
================================================================

DATASET 16: Consumer Loan Applications and Default Outcomes
Source:    Kaggle — Home Credit Default Risk Competition
Portal:    kaggle.com/c/home-credit-default-risk
File:      homecredit_application_train_raw.csv
Records:   307,511 loan applications
License:   Competition dataset
           Permitted for educational and non-commercial use
Geography: Eastern Europe and Southeast Asia
           NOT Kenya — calibration required

CALIBRATION NOTE:
This dataset is used as a behavioural proxy only.
It is not representative of Kenyan borrowers.
Probability of default outputs are calibrated to
Kenya-specific NPL levels using CBK and World Bank
Financial Soundness Indicator data.
The full calibration methodology is documented in:
notebooks/02_modeling.ipynb

No proprietary or personally identifiable borrower
data was used anywhere in this analysis.

DATASET 17: Credit Bureau History
Source:    Kaggle — Home Credit Default Risk Competition
File:      homecredit_bureau_raw.csv
Records:   1,716,428 bureau entries
License:   Competition dataset
Geography: Eastern Europe and Southeast Asia
Use:       Behavioural feature engineering —
           previous default history,
           outstanding balance aggregation

================================================================
SECTION 5 — PROXY AND SUBSTITUTION LOG
================================================================

The following substitutions were made where primary sources
were unavailable. All substitutions are documented and
disclosed in the investment memo methodology section.

Primary Source     | Unavailable Reason       | Proxy Used
-------------------|--------------------------|------------------
KNBS Unemployment  | No CSV download          | ILO Modelled Est.
KNBS Inflation     | No CSV download          | World Bank CPI
KNBS GDP Growth    | No CSV download          | World Bank GDP
KNBS Population    | No CSV download          | World Bank Pop.
KNBS Income        | No structured download   | Analyst-constructed
CBK NPL Ratio      | Portal navigation issue  | World Bank FSI
CBK GDP Per Capita | Wrong file downloaded    | Derived from WB GDP

================================================================
SECTION 6 — GENERAL DISCLAIMER
================================================================

All data used in this project is sourced from publicly
available portals and is used for educational and research
purposes only.

This analysis does not constitute investment advice.
No real capital deployment decisions should be made
solely on the basis of this analysis.

All modelling assumptions are documented in the
methodology.md file in the docs/ folder.

This project is intended to demonstrate analytical
capability for professional portfolio purposes.

================================================================
END OF DATA USAGE DOCUMENTATION
================================================================