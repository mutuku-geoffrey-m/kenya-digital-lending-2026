# Kenya Digital Lending — Investment Due Diligence
### Full-Stack Investment Analysis | February 2026

**Analyst:** Geoffrey Mutuku  
**Scope:** End-to-end investment due diligence on a Kenyan digital consumer lending platform  
**Decision Framework:** Base IRR > 25% | Recession IRR > 10% | Capital loss probability < 20%  
**Recommendation:** INVEST — All three decision criteria pass across 10,000 Monte Carlo simulations

---

## Interactive Dashboard

**[View Live Dashboard on Tableau Public →](https://public.tableau.com/app/profile/geoffrey.mutuku/viz/kenya_digital_lending_2026/01MarketOpportunity)**

### Dashboard 1 — Market Opportunity
- Kenya interest rate environment and NPL ratio 2014–2025
- M-Pesa ecosystem growth FY2020–FY2025
- TAM/SAM/SOM market opportunity funnel — 19.2M digitally reachable borrowers

### Dashboard 2 — Investment Returns
- Scenario IRR comparison across 4 historical Kenya economic events
- Monte Carlo IRR distribution across 10,000 simulations
- Investment decision scorecard — all 6 criteria pass

---

## Key Results

| Metric | Value |
|--------|-------|
| Best ML model | Gradient Boosting |
| Model AUC | 0.7396 |
| Calibration target | Kenya CBK NPL 12.34% (2023) |
| Monte Carlo simulations | 10,000 paths |
| Median IRR | 86.7% |
| 5th percentile IRR | 65.1% |
| Capital loss probability | 0.0% |
| Severe recession IRR | 27.2% |
| Overall recommendation | **INVEST** |

---

## Project Structure

```
kenya-digital-lending-2026/
├── notebooks/
│   ├── 01_data_cleaning_macro.ipynb       # Macro panel — 143 months 2014–2025
│   ├── 02_digital_ecosystem.ipynb         # M-Pesa metrics and TAM/SAM/SOM model
│   ├── 03_borrower_risk_model.ipynb       # Gradient Boosting PD model
│   └── 04_stress_testing.ipynb            # Monte Carlo simulation
├── excel/
│   └── investment_model.xlsx              # 8-sheet investment model
├── tableau/
│   └── kenya_digital_lending_2026.twbx    # Tableau workbook
├── data/
│   ├── raw/                               # Source files — stored on Google Drive
│   └── clean/                             # Model-ready CSV outputs
├── outputs/
│   └── charts/                            # Python-generated charts
└── docs/
    └── data_usage.txt                     # Full data source documentation
```

---

## What Was Built

### Python Risk Model — 4 Notebooks

**Notebook 01 — Macro Data Cleaning**
Cleaned 15 raw datasets from CBK, World Bank, ILO and IMF. Built unified monthly macro panel covering 143 months from January 2014 to November 2025. Output: `macro_panel_monthly.csv` with 17 columns including lending rates, NPL ratio, GDP growth, inflation, unemployment, private credit and engineered stress features.

**Notebook 02 — Digital Ecosystem and Market Sizing**
Cleaned Safaricom M-Pesa metrics FY2020–FY2025. Built TAM/SAM/SOM model anchored to population and M-Pesa penetration data. M-Pesa penetration at 101% of adult population confirms digital distribution infrastructure is already built. Output: TAM 20.0M, SAM 19.2M, SOM 576K target borrowers.

**Notebook 03 — Borrower Risk Model**
Trained Logistic Regression, Random Forest and Gradient Boosting on 307,511 Home Credit loan applications. Gradient Boosting selected with AUC 0.7396. Calibrated model outputs to Kenya CBK NPL ratio using Platt scaling. Calibration factor 0.994x — near perfect alignment to Kenya base rate.

Segment PDs calibrated to Kenya:
| Segment | PD | LGD | Recommended APR |
|---------|-----|-----|----------------|
| Prime | 3.20% | 35% | ~31% |
| Near Prime | 7.70% | 45% | ~37% |
| Subprime | 20.06% | 60% | ~48% |

**Notebook 04 — Stress Testing and Monte Carlo**
Calibrated macro elasticities from 10 years of CBK NPL historical data. Ran 10,000 Monte Carlo simulations drawing random macro shocks from historical distributions. Capital loss probability 0.0% across all paths. Tested 4 historical Kenya scenarios anchored to 2024 baseline, 2017 drought, 2008 post-election crisis and 2016 rate cap.

---

### Excel Investment Model — 8 Sheets

| Sheet | Purpose |
|-------|---------|
| ASSUMPTIONS | 50 named parameters across 5 blocks — single source of truth |
| MARKET_MODEL | 36-month borrower acquisition and loan origination forecast |
| RISK_SEGMENTS | PD, LGD and breakeven APR by Prime, Near Prime, Subprime |
| LOAN_CASHFLOWS | Single cohort amortisation — verified IRR 57%, MOIC 1.11 |
| PORTFOLIO | 36-month loanbook roll-forward with revenue and cost flows |
| INCOME_STATEMENT | 3-year P&L — net margin approximately 46–48% |
| INVESTOR_RETURNS | Equity IRR, MOIC, DPI, TVPI and 6-criteria decision box |
| STRESS_TEST | 4 scenarios with stressed PD, LGD, APR and IRR outcomes |

---

## Market Thesis

Kenya is one of the most compelling digital lending markets globally for three structural reasons.

**First — infrastructure already built.** M-Pesa penetration stands at 101% of the adult population with FY2025 transaction value of KES 38,290B across 35.8M active users. A digital lender does not need to build distribution — it needs to plug into an existing financial operating system.

**Second — credit gap is large.** Kenya's domestic credit to private sector stands at approximately 32% of GDP against a global average of approximately 90%. This 58 percentage point gap represents a structural underserved demand for credit among working-age adults who have mobile money access but no formal credit history.

**Third — macro environment supports lending.** CBK policy rate and commercial lending rates provide a viable spread for digital lenders operating with technology-driven cost efficiency. Despite elevated NPLs at system level (12.34% in 2023), short-duration digital loans with behavioural scoring demonstrate significantly lower loss rates than the system average.

---

## Stress Test Summary

| Scenario | Historical Precedent | Portfolio PD | Gross IRR | Verdict |
|----------|---------------------|-------------|-----------|---------|
| Base Case | Kenya 2024 baseline | 8.2% | 102.4% | INVEST |
| Mild Recession | Kenya 2017 drought | 14.6% | 57.5% | PROCEED |
| Severe Recession | Kenya 2008 crisis | 23.5% | 27.2% | ACCEPTABLE |
| APR Cap Shock | Kenya 2016 rate cap | 8.2% | 76.5% | MANAGEABLE |

All four scenarios clear the 10% minimum return floor. The investment thesis holds even under the most severe historical stress scenario Kenya has experienced in the past 20 years.

---

## Key Assumptions and Known Limitations

**On the base case IRR:**
The gross IRR of 102% reflects loan-level economics driven by upfront origination fees on short-duration 3-month instruments. A 6% origination fee annualises to approximately 24% on its own. Equity-level returns to investors are moderated by customer acquisition costs, operating overhead and idle capital costs. A conservative 5x EBITDA exit multiple scenario (versus 8x base case) produces gross IRR of approximately 55–65% — still substantially above the 25% hurdle.

**On the NPL ratio:**
The monthly portfolio NPL ratio of approximately 0.61% reflects the flow dynamics of a 3-month loan portfolio. Rapid loan turnover means defaults are recognised and written off within the quarter they occur. This is mechanically distinct from the CBK system-level NPL ratio which accumulates across multi-year loan books. The annualised default rate of 8.6% is consistent with Kenya digital lending benchmarks.

**On the DPI metric:**
Returns are weighted toward the terminal exit. Early-stage digital lenders typically reinvest operating cashflows into portfolio growth rather than distributing dividends. The model accurately flags this structure — investors should underwrite to a conservative exit multiple and negotiate exit triggers at term sheet stage.

**On the borrower data:**
The Home Credit dataset covers Eastern Europe and Southeast Asia borrowers — not Kenya. PD outputs are calibrated to Kenya NPL levels but behavioural features are not directly transferable. Model outputs should be treated as directional estimates pending access to Kenya-specific credit bureau data from TransUnion Kenya or Metropol CRB.

---

## Data Sources

| Source | Dataset | Frequency | Use |
|--------|---------|-----------|-----|
| Central Bank of Kenya | Lending rates, policy rate, private credit | Monthly | Interest rate environment |
| World Bank Open Data | NPL ratio, GDP, inflation, population | Annual | Macro panel |
| IMF Financial Access Survey | Mobile money penetration | Annual | Digital ecosystem |
| Safaricom Annual Reports | M-Pesa metrics FY2020–FY2025 | Annual | Market sizing |
| ILO Labour Statistics | Kenya unemployment modelled estimates | Annual | Macro stress |
| Home Credit Default Risk (Kaggle) | 307,511 loan applications | Cross-sectional | PD model training |

Full data source documentation including substitution log and proxy methodology is in `docs/data_usage.txt`.

---

## Tools and Technologies

| Tool | Version | Use |
|------|---------|-----|
| Python | 3.x | Data cleaning, ML modelling, Monte Carlo |
| Google Colab | — | Notebook execution environment |
| scikit-learn | Latest | Logistic Regression, Random Forest, Gradient Boosting |
| pandas / numpy | Latest | Data manipulation and numerical computing |
| matplotlib | Latest | Chart generation |
| Microsoft Excel | 365 | 8-sheet investment model |
| Tableau Public | Latest | Interactive dashboard |
| GitHub Desktop | Latest | Version control |

---

## Disclaimer

This analysis is produced for educational and portfolio demonstration purposes only. It does not constitute investment advice. No real capital deployment decisions should be made solely on the basis of this analysis. All modelling assumptions are documented and disclosed. The Home Credit dataset is used under Kaggle competition terms for non-commercial educational use only.

---

*Built by Geoffrey Mutuku | February 2026 | Kenya Digital Lending Investment Due Diligence*
