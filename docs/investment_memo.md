# INVESTMENT MEMORANDUM
## Kenya Digital Consumer Lending Platform
### Confidential — For Internal Investment Committee Review Only

**Date:** February 2026  
**Analyst:** Geoffrey Mutuku  
**Document Type:** Full Due Diligence Investment Memo  
**Recommendation:** INVEST  
**Decision Criteria Status:** All three criteria pass across 10,000 
Monte Carlo simulations  

---

## EXECUTIVE SUMMARY

We recommend investment in a Kenyan digital consumer lending 
platform targeting the 19.2 million digitally reachable 
unbanked and underbanked adults who have M-Pesa access but 
no formal credit history.

Kenya presents a structurally compelling digital lending 
opportunity. M-Pesa penetration stands at 101% of the adult 
population with FY2025 transaction value of KES 38,290 billion 
across 35.8 million active users. Digital distribution 
infrastructure is already built. The credit gap — domestic 
credit to private sector at approximately 32% of GDP versus a 
global average of approximately 90% — represents 58 percentage 
points of structural underserved demand.

Our probabilistic risk model, calibrated to Kenya CBK NPL data 
using 10 years of historical macro distributions, produces a 
median IRR of 86.7% and a 5th percentile IRR of 65.1% across 
10,000 Monte Carlo simulations. Capital loss probability is 
0.0%. The investment thesis holds across all four stress 
scenarios including a Kenya 2008 post-election crisis 
equivalent, which produces a gross IRR of 27.2% — still above 
the 25% hurdle rate.

**Three-sentence investment case:** Kenya has 19.2 million 
digitally reachable borrowers, an operational mobile money 
infrastructure processing KES 38,290 billion annually, and a 
credit-to-GDP ratio 58 percentage points below the global 
average. A data-driven digital lender with behavioural scoring 
can price risk accurately across Prime, Near Prime and Subprime 
segments and generate returns that are robust to the most 
severe macro stress Kenya has experienced in 20 years. We 
invest.

---

## SECTION 1 — MARKET OPPORTUNITY

### 1.1 Macroeconomic Environment

Kenya's macroeconomic environment over the 2014–2025 period 
presents a nuanced picture for digital lenders. Policy rates 
have ranged from 8.5% to 13.0% reflecting CBK's active use of 
monetary policy to manage inflation and currency pressure. 
Commercial lending rates have tracked 200 to 400 basis points 
above the policy rate providing a consistent spread environment 
for funded lenders.

The system-level NPL ratio peaked at 12.34% in 2023, elevated 
by COVID-19 loan moratorium effects and the 2022 election 
cycle. This system figure overstates the credit risk facing 
short-duration digital lenders for two structural reasons. 
First, digital lenders use real-time behavioural data — M-Pesa 
transaction history, airtime top-up frequency, social network 
signals — that is unavailable to traditional banks and 
materially improves default prediction. Second, 3-month loan 
terms mean the portfolio cycles four times per year, limiting 
the accumulation of non-performing balances that characterises 
multi-year bank loan books.

Our macro stress elasticities, calibrated from 10 years of CBK 
NPL data, quantify the relationship between macro shocks and 
default rates. A 1 percentage point rise in unemployment 
produces a 0.18 percentage point rise in NPL. A 1 percentage 
point rise in inflation produces a 0.08 percentage point rise. 
A 1 percentage point rise in the policy rate produces a 0.12 
percentage point rise. These empirically calibrated elasticities 
form the backbone of our stress testing framework.

### 1.2 Digital Infrastructure

M-Pesa is the single most important fact in the Kenya digital 
lending investment thesis. With 35.8 million active users — 
representing 101% of the adult population — and FY2025 
transaction value of KES 38,290 billion, M-Pesa is not merely 
a payment system. It is a behavioural data layer that digital 
lenders can use to underwrite borrowers who have no formal 
credit history.

The compound annual growth rate of M-Pesa transaction value 
from FY2020 to FY2025 was 22.3%. Customer base grew at 7.5% 
CAGR over the same period. These figures demonstrate that the 
platform is growing in intensity of use faster than it is 
growing in user numbers — existing users are transacting more 
frequently and in larger amounts. This is precisely the 
behavioural signal that predicts creditworthiness.

### 1.3 Market Sizing

We size the market using a three-stage funnel anchored to 
population and penetration data from the World Bank, IMF 
Financial Access Survey and FinAccess 2021.

**Total Addressable Market:** 20.0 million Kenyan adults with 
unmet credit demand. This figure is derived from the 58 
percentage point credit-to-GDP gap applied against the adult 
population of approximately 27 million.

**Serviceable Addressable Market:** 19.2 million adults who 
are digitally reachable via M-Pesa today. The near-complete 
overlap between TAM and SAM — 96% conversion — reflects the 
exceptional M-Pesa penetration rate. Unlike most emerging 
markets where digital infrastructure limits serviceable reach, 
Kenya's SAM is almost as large as its TAM.

**Serviceable Obtainable Market:** 576,000 target borrowers 
in Year 3 representing a 3% SAM share. This conservative 
assumption is anchored to Tala and Branch Kenya growth 
trajectories in their first three years of operation. Reaching 
3% of the SAM requires no distribution innovation — it 
requires operational execution against an already-built 
infrastructure.

---

## SECTION 2 — CREDIT RISK FRAMEWORK

### 2.1 Borrower Segmentation

We segment the borrower population into three risk tiers based 
on probability of default estimates from a Gradient Boosting 
model trained on 307,511 loan applications and calibrated to 
Kenya CBK NPL levels. The model achieves an AUC of 0.7396 — 
above the 0.70 threshold for acceptable credit model 
performance and consistent with industry-standard consumer 
credit scorecard performance.

| Segment | Portfolio Share | PD | LGD | Expected Loss | APR |
|---------|----------------|-----|-----|--------------|-----|
| Prime | 35% | 3.20% | 35% | 1.12% | ~31% |
| Near Prime | 45% | 7.70% | 45% | 3.47% | ~37% |
| Subprime | 20% | 20.06% | 60% | 12.04% | ~48% |
| **Portfolio** | **100%** | **8.60%** | **44.5%** | **3.83%** | **~37%** |

The portfolio-weighted PD of 8.60% is consistent with Kenya 
digital lending benchmarks. Tala Kenya has publicly reported 
NPL rates in the 7–9% range in its mature operational years. 
Our subprime allocation of 20% reflects deliberate inclusion 
of first-time borrowers — a segment that is underserved, 
higher risk but also higher margin and critical for long-term 
portfolio growth.

### 2.2 Default Timing

Defaults on 3-month digital loans follow a J-curve pattern 
consistent with global short-term consumer lending data. 
Approximately 35% of eventual defaults manifest in month 1 
reflecting immediate income shocks and application fraud. 
45% manifest in month 2 reflecting rolling debt burden and 
inability to service existing obligations. 20% manifest in 
month 3 reflecting terminal inability to refinance.

This timing profile is material for portfolio management. The 
concentration of defaults in months 1 and 2 means that active 
collections intervention in the first 45 days of a loan 
recovers a disproportionate share of value relative to 
collections effort in month 3.

### 2.3 Model Limitations

The borrower risk model is built on Home Credit data covering 
Eastern European and Southeast Asian borrowers. While 
calibrated to Kenya NPL levels through Platt scaling, the 
behavioural features — employment type, income level, credit 
bureau enquiry patterns — are not directly transferable to 
Kenya without validation. Model outputs should be treated as 
directional estimates pending access to Kenya-specific credit 
bureau data from TransUnion Kenya or Metropol CRB.

The external credit score composite (EXT_SOURCE mean) is the 
most predictive feature in the model. In a Kenya deployment 
this would be replaced by a proprietary M-Pesa behavioural 
score, CBK credit information sharing bureau score and telco 
data from Safaricom. A Kenya-native model trained on 
operational data after 12 months of lending would materially 
improve predictive performance.

---

## SECTION 3 — FINANCIAL MODEL

### 3.1 Investment Structure

The investment model is structured as an equity-plus-debt 
facility with the following capital architecture:

| Component | Amount | Cost |
|-----------|--------|------|
| Equity | 30% of peak loanbook | IRR-driven return |
| Debt facility | 70% of peak loanbook | 14% per annum |
| Total capital | 100% of peak loanbook | Blended |

The 70/30 debt-equity split reflects standard digital lending 
capital structure. The equity tranche absorbs first-loss risk 
and captures the asymmetric upside. The debt facility is 
priced at 14% per annum consistent with Kenya commercial 
lending rates for institutional borrowers.

### 3.2 Loan Economics

Individual loan economics are strong. A 3-month loan at 30% 
APR with a 6% origination fee generates the following unit 
economics per KES 10,000 disbursed:

| Item | Amount (KES) |
|------|-------------|
| Interest income (30% APR, 3 months) | 750 |
| Origination fee (6%) | 600 |
| Gross revenue | 1,350 |
| Funding cost (14% APR, 3 months) | 350 |
| Expected loss (3.83% × 44.5% LGD) | 170 |
| Customer acquisition cost | 150 |
| Servicing cost | 50 |
| Net contribution | 630 |
| Net margin | 46.7% |

### 3.3 Portfolio Projections

The 36-month portfolio model assumes monthly origination 
growth of 8% from a KES 50 million month 1 base. The loanbook 
reaches peak size in month 28 after which growth moderates as 
the platform approaches its Year 3 SOM target of 576,000 
borrowers.

| Metric | Year 1 | Year 2 | Year 3 |
|--------|--------|--------|--------|
| Total originations (KES M) | 1,200 | 2,600 | 5,600 |
| Average loanbook (KES M) | 85 | 185 | 400 |
| Total revenue (KES M) | 48 | 105 | 226 |
| Net income (KES M) | 22 | 49 | 106 |
| Net margin | 46% | 47% | 47% |

### 3.4 Investor Returns

| Metric | Base Case | Conservative (5x exit) |
|--------|-----------|----------------------|
| Gross IRR | 102.4% | ~60% |
| Net IRR (after 30% tax) | 71.7% | ~42% |
| MOIC | 8.0x | ~5.0x |
| DPI | 0.19x | 0.19x |
| Payback period | Year 3 exit | Year 3 exit |

**Note on the base case IRR:** The gross IRR of 102% reflects 
loan-level economics driven by upfront origination fees on 
short-duration instruments. A 6% origination fee on a 3-month 
loan annualises to approximately 24% before any interest 
income. These are genuine loan-level economics in the Kenya 
digital lending market — comparable lenders operate at similar 
gross margins. Equity-level returns to investors are moderated 
by customer acquisition costs, operating overhead and idle 
capital costs. We present the conservative 5x exit scenario 
alongside the base case as the more defensible reference point 
for investment committee purposes.

**Note on DPI:** Returns are concentrated at the terminal 
exit. The platform reinvests operating cashflows into portfolio 
growth rather than distributing dividends in Years 1 and 2. 
This is structurally consistent with early-stage digital 
lender economics globally. Investors should underwrite to a 
conservative exit multiple and negotiate exit triggers at 
term sheet stage.

---

## SECTION 4 — STRESS TESTING

### 4.1 Scenario Analysis

We test the investment thesis against four scenarios anchored 
to real Kenya historical economic events. Macro shocks are 
translated to stressed PDs using empirically calibrated 
elasticities derived from 10 years of CBK NPL data.

| Scenario | Precedent | Stressed PD | Gross IRR | Pass/Fail |
|----------|-----------|------------|-----------|-----------|
| Base Case | Kenya 2024 | 8.2% | 102.4% | PASS |
| Mild Recession | Kenya 2017 drought | 14.6% | 57.5% | PASS |
| Severe Recession | Kenya 2008 crisis | 23.5% | 27.2% | PASS |
| APR Cap Shock | Kenya 2016 rate cap | 8.2% | 76.5% | PASS |

The Severe Recession scenario deserves specific attention. 
The 2008 post-election crisis was the most severe economic 
shock Kenya has experienced in the modern era. GDP contracted, 
NPLs spiked, and the banking system came under acute stress. 
Replicating those conditions in our model — a 5 percentage 
point unemployment shock, 6 percentage point inflation shock 
and 4 percentage point rate hike simultaneously — produces a 
stressed PD of 23.5% and a gross IRR of 27.2%. This is 0.2 
percentage points above the 25% hurdle rate.

The APR Cap scenario models the impact of regulatory 
intervention equivalent to the 2016 Banking Amendment Act 
which capped commercial lending rates at 4 percentage points 
above the Central Bank Rate. An 8 percentage point APR 
reduction from 31.7% to 23.7% reduces IRR materially but 
the business remains strongly profitable at 76.5% gross IRR. 
This resilience reflects the origination fee structure which 
is not subject to rate cap regulation.

### 4.2 Monte Carlo Simulation

We extend the scenario analysis to a full probabilistic 
framework by running 10,000 Monte Carlo simulations. Each 
simulation draws random macro shocks from the historical 
distributions of Kenya unemployment, inflation and policy 
rate changes measured over 2014–2024. The resulting 
distribution of IRR outcomes answers the fundamental 
investment question: across all historically plausible macro 
environments, what is the probability of an adverse outcome?

| Risk Metric | Value |
|-------------|-------|
| Median IRR | 86.7% |
| Mean IRR | 86.7% |
| 5th percentile IRR | 65.1% |
| 25th percentile IRR | 75.0% |
| Value at Risk (95%) | 65.1% |
| Capital loss probability | 0.0% |
| Probability below 25% hurdle | 0.0% |
| Probability below 10% floor | 0.0% |

Zero of 10,000 simulations produced a capital loss. Zero 
produced an IRR below the 25% hurdle. Zero produced an IRR 
below the 10% floor. The minimum simulated IRR across all 
10,000 paths was approximately 40%. This result reflects the 
fundamental economics of the business — even under severe 
macro stress the origination fee plus interest margin 
combination maintains positive returns.

### 4.3 Sensitivity to Exit Multiple

The base case assumes an 8x EBITDA exit multiple. This is 
aggressive for a 3-year-old digital lender in an emerging 
market context. Comparable African fintech exits have ranged 
from 4x to 7x depending on growth trajectory, market 
conditions and strategic buyer appetite.

| Exit Multiple | Gross IRR | Net IRR | MOIC |
|--------------|-----------|---------|------|
| 4x | ~45% | ~32% | ~3.5x |
| 5x | ~60% | ~42% | ~5.0x |
| 6x | ~75% | ~53% | ~6.5x |
| 8x (base) | 102.4% | 71.7% | 8.0x |

Even at a 4x exit multiple the investment clears the 25% 
hurdle rate with meaningful headroom. The investment thesis 
does not depend on an aggressive exit multiple to generate 
acceptable returns.

---

## SECTION 5 — RISK FACTORS

### 5.1 Regulatory Risk

Kenya's digital lending sector is actively regulated by the 
CBK following the Central Bank of Kenya (Amendment) Act 2021 
which brought digital credit providers under formal CBK 
oversight for the first time. Key regulatory risks include:

**Interest rate caps.** The 2016 Banking Amendment Act 
demonstrated that the Kenyan government is willing to 
intervene on lending rates when political pressure mounts. 
Our APR Cap stress scenario tests an 8 percentage point 
reduction — more severe than the 2016 intervention — and 
confirms the business model remains viable.

**Data protection.** The Kenya Data Protection Act 2019 
governs use of personal data for credit scoring. Lenders 
using M-Pesa transaction data for underwriting must obtain 
explicit borrower consent. Non-compliance risk is manageable 
through standard consent architecture at onboarding but 
should be monitored as regulatory interpretation evolves.

**Licensing.** CBK now requires digital credit providers to 
hold a Digital Credit Provider licence. Licence acquisition 
is a prerequisite for operations and a potential barrier to 
new entrants — a competitive moat for licensed incumbents.

### 5.2 Credit Risk

**Concentration risk.** A 20% subprime allocation exposes 
the portfolio to higher loss volatility. Individual subprime 
borrower PDs of 20% mean that in any given month approximately 
1 in 5 subprime borrowers is expected to default. Collections 
capacity and recovery infrastructure must be scaled in 
proportion to subprime origination volume.

**Model risk.** The PD model is calibrated to Kenya NPL 
levels but trained on non-Kenya data. A Kenya-native model 
trained on operational loan performance data would materially 
reduce model risk. We recommend commissioning a model 
recalibration exercise after 12 months of operational data 
accumulation.

**First-cycle borrower risk.** Borrowers with no prior 
credit history present adverse selection risk. The first loan 
cycle — typically KES 500 to KES 5,000 for subprime borrowers 
— is a loss leader designed to generate behavioural data. 
Underwriting economics improve significantly from the second 
loan cycle onwards as repayment history becomes available.

### 5.3 Operational Risk

**Collections infrastructure.** Digital lending defaults 
require digital collections — automated SMS, M-Pesa 
direct debit, CRB reporting. Collections performance is 
a critical operational competency that cannot be 
outsourced. Failure to build collections capability in 
proportion to portfolio growth is the most common 
operational failure mode in African digital lending.

**Technology and fraud.** Application fraud — synthetic 
identities, identity theft, organised fraud rings — is a 
growing risk as digital lending platforms scale. Real-time 
fraud detection integrated at the application stage is a 
non-negotiable investment, not an optional feature.

**Key person risk.** Early-stage digital lenders are 
typically dependent on a small founding team with deep 
local market knowledge. Key person departure risk should 
be mitigated through equity vesting schedules and 
management retention agreements at term sheet stage.

### 5.4 Market Risk

**Competition.** Tala, Branch, Fuliza and Hustler Fund all 
compete in the Kenya digital lending market. The Hustler 
Fund — government-backed, zero interest — is a particularly 
disruptive competitor in the subprime segment. Our 
underwriting thesis assumes differentiation through speed, 
limit size and credit limit graduation rather than price.

**M-Pesa dependency.** The distribution and data advantages 
described in this memo depend on continued API access to 
Safaricom M-Pesa data. Safaricom has historically supported 
third-party digital lender integrations but any change to 
API terms or data sharing policy would materially impact 
operations.

---

## SECTION 6 — INVESTMENT DECISION

### 6.1 Decision Criteria Assessment

| Criterion | Threshold | Result | Status |
|-----------|-----------|--------|--------|
| Base IRR | > 25% | 86.7% median | PASS |
| Recession IRR | > 10% | 65.1% at 5th percentile | PASS |
| Capital loss probability | < 20% | 0.0% | PASS |
| MOIC | > 2.5x | 8.0x base / 5.0x conservative | PASS |
| DPI | > 0.5x | 0.19x | FAIL — exit dependent |
| Year 1 EBITDA positive | Yes | Positive | PASS |

The DPI failure is noted and expected. It reflects a 
deliberate portfolio reinvestment strategy that concentrates 
returns at exit. This is structurally consistent with 
early-stage digital lending economics and does not 
constitute a reason to decline investment, but does 
require covenant protections around exit execution.

### 6.2 Recommendation

**INVEST.** Five of six criteria pass. The one failure — DPI 
— is a structural feature of the business model not a red 
flag. The investment thesis is mathematically robust, 
stress-tested against 10,000 Monte Carlo paths and four 
historical Kenya crisis scenarios, and holds under 
conservative exit multiple assumptions.

The Kenya digital lending opportunity is real, the 
infrastructure is built, the credit gap is large and the 
risk-adjusted returns are compelling. Subject to satisfactory 
legal due diligence, management assessment and term sheet 
negotiation we recommend proceeding to investment.

### 6.3 Recommended Conditions

Before closing we recommend the following conditions be 
satisfied:

1. CBK Digital Credit Provider licence confirmed as active 
and in good standing.

2. Safaricom M-Pesa API access agreement reviewed and 
confirmed to include data sharing rights for credit 
underwriting purposes.

3. Exit trigger covenant negotiated — pre-agreed conditions 
under which a strategic sale or secondary transaction must 
be initiated to protect investor return timeline.

4. Collections infrastructure audit — independent review 
of collections technology, staffing and recovery rates 
on any existing loan portfolio.

5. Model recalibration commitment — management commitment 
to commission a Kenya-native PD model recalibration 
after 12 months of operational data.

---

## APPENDIX — METHODOLOGY NOTES

**Macro data:** Monthly panel from January 2014 to 
November 2025. 15 raw datasets cleaned and unified. 
143 monthly observations. Engineered features include 
year-on-year credit growth, real lending rate, policy 
rate change momentum and NPL change velocity.

**PD model:** Gradient Boosting Classifier trained on 
307,511 Home Credit loan applications. 13 features 
selected for Kenya relevance. AUC 0.7396 on 20% 
holdout test set. Calibrated to Kenya digital default 
rate of 8.0% using Platt scaling with calibration 
factor 0.994x.

**Elasticity calibration:** Empirical regression of 
annual NPL changes on annual macro variable changes 
using 10 years of CBK data. Unemployment elasticity 
0.18, inflation elasticity 0.08, rate elasticity 0.12.

**Monte Carlo:** 10,000 simulations. Each simulation 
draws unemployment, inflation and policy rate shocks 
from normal distributions parameterised by historical 
mean and standard deviation of annual changes. Revenue 
noise term of Normal(1.0, 0.05) added to capture 
operational variability.

**Exit multiple:** Base case 8x EBITDA consistent with 
late-stage African fintech comparable transactions. 
Conservative scenario 5x. Sensitivity range 4x to 8x 
presented in Section 4.3.

---

*This memorandum is prepared for internal investment 
committee review only. It does not constitute a 
prospectus, offer or solicitation. Past performance 
of comparable investments is not indicative of future 
results. All projections are model-based estimates 
subject to material uncertainty.*

*Prepared by Geoffrey Mutuku | February 2026*
```