# Bank Loan Approval Analysis
 
![Python](https://img.shields.io/badge/Python-3.x-blue) ![Pandas](https://img.shields.io/badge/Pandas-Data%20Wrangling-lightgrey) ![Matplotlib](https://img.shields.io/badge/Matplotlib-Visualisation-orange)
 
---
 
## Business Question
 
> **What applicant characteristics most reliably predict loan default risk — and how can lenders use this to reduce bad debt while staying fair?**
 
Credit risk is the foundation of retail banking and fintech lending. Every loan approval decision carries financial risk — and lenders who can't accurately identify default-prone applicants either lose money on bad debt or lose customers through over-cautious rejections. This project explored what the data actually reveals about which applicant factors matter most, and what that means for lending strategy.
 
---
 
## The Data Challenge
 
Real loan datasets carry significant messiness — missing credit history entries, income figures that appear as outliers but are legitimate, and categorical variables encoded inconsistently across records. A key decision in this project was how to treat missing credit history: imputing it vs flagging it as a risk signal in its own right. I treated absence of credit history as a meaningful data point rather than a gap to fill — a deliberate analytical choice that changed the risk distribution.
 
---
 
## Method
 
- Loaded and explored loan applicant dataset — profiled distributions across income, loan amount, credit history, employment status, and dependents
- Cleaned data: handled missing values with domain-informed decisions, standardised categorical variables, removed duplicate applicant records
- Performed feature analysis — examined approval rate and default rate across each variable independently and in combination
- Visualised risk distributions using Matplotlib — approval rate by credit history, income band, loan-to-income ratio, and employment type
- Identified the variables with strongest predictive signal for both approval likelihood and default risk
---
 
## What I Found
 
- **Credit history** was the single strongest predictor of both approval and default — applicants with no credit history defaulted at more than 3x the rate of those with established history
- **Loan-to-income ratio** was a stronger risk signal than loan amount alone — high earners taking large loans were lower risk than moderate earners taking the same absolute amount
- **Employment type** mattered more than employment duration — self-employed applicants showed higher default rates regardless of income level, suggesting lenders price this risk inconsistently
- Married applicants with dependents showed unexpectedly lower default rates when controlling for income — a counterintuitive finding worth further investigation
---
 
## Business Recommendation
 
For a credit risk team or lending strategy function:
 
1. **Loan-to-income ratio should be a primary screening variable** — not just loan amount. The data shows this is more predictive and more equitable than absolute income thresholds
2. Self-employed applicants warrant a differentiated risk model — applying salaried-employee criteria to this segment likely misprices risk in both directions
3. Credit history absence should trigger a verification step, not automatic rejection — the risk is real but the population is not homogeneous
---
 
## How To Run
 
```bash
git clone https://github.com/YashviPandya/Bank_Loan_Approval_Data_Project.git
cd Bank_Loan_Approval_Data_Project
pip install pandas matplotlib
jupyter notebook
```
 
---
 
## Skills Demonstrated
 
`Exploratory data analysis` · `Feature analysis` · `Risk segmentation` · `Domain-informed data cleaning` · `Financial services context` · `Python` · `Pandas` · `Matplotlib` · `Business recommendation`
