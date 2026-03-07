# 🏦 Bank Loan Approval Analysis & Predictive Modelling

![Python](https://img.shields.io/badge/Python-3.9-blue) ![Jupyter](https://img.shields.io/badge/Notebook-Jupyter-orange) ![ML](https://img.shields.io/badge/ML-Classification-red) ![Status](https://img.shields.io/badge/Status-Complete-brightgreen)

## 📌 Business Question
> **Which applicant profiles are most likely to default — and can we build a model that helps loan officers make faster, fairer, and more accurate approval decisions?**

Loan default costs UK banks billions annually. Manual review processes are slow and inconsistent. A data-driven approval model reduces risk exposure and speeds up decisions for creditworthy applicants.

---

## 📊 Project Overview

This project analyses bank loan approval data using Python to identify the key drivers of loan approval and default risk. It combines **exploratory data analysis** with a **predictive classification model** to help financial institutions make better lending decisions.

**Tools Used:** Python (Pandas, NumPy, Matplotlib, Seaborn, Scikit-learn) · Jupyter Notebook

---

## 🔍 Key Findings from EDA

- **Credit history is the dominant factor:** Applicants with a positive credit history were approved at an 80% rate vs 10% for those without — by far the strongest predictor
- **Income threshold effect:** Applicants with combined household income above £45,000 saw approval rates jump from 58% to 79%, suggesting an implicit income threshold in decision-making
- **Property area impact:** Semi-urban applicants had the highest approval rates (76%), outperforming both urban (68%) and rural (61%) applicants
- **Gender gap identified:** Male applicants were approved at a 70% rate vs 65% for female applicants with comparable financial profiles — a potential bias flag for compliance review

---

## 🤖 Predictive Model

A **Logistic Regression classifier** was trained to predict loan approval outcomes:

| Metric | Score |
|--------|-------|
| Accuracy | 82% |
| Precision | 84% |
| Recall | 79% |
| F1 Score | 81% |

**Top predictive features:** Credit history · Applicant income · Loan amount term · Property area

---

## 💡 Business Recommendation

1. **Automate low-risk approvals:** Applicants meeting all top-3 predictor thresholds (clean credit history, income >£45K, semi-urban property) can be auto-approved with high confidence, reducing manual review time by an estimated 40%
2. **Flag potential bias:** The gender disparity in approval rates warrants a fairness audit — controlling for income and credit score, approval rates should be equalised
3. **Model deployment:** This logistic regression model is suitable for a pilot deployment as a scoring tool to assist (not replace) loan officers in initial screening

---

## 📁 Repository Structure

```
├── data/
│   └── loan_data.csv
├── notebooks/
│   └── bank_loan_analysis.ipynb
├── models/
│   └── loan_approval_model.pkl
└── README.md
```

---

## 🚀 How to Run

```bash
git clone https://github.com/YashviPandya/Bank_Loan_Approval_Data_Project
pip install pandas numpy matplotlib seaborn scikit-learn
jupyter notebook notebooks/bank_loan_analysis.ipynb
```

---

## 📬 Contact
**Yashvi Pandya** · [LinkedIn](http://www.linkedin.com/in/yashvipandya) · MSc Data Analytics
