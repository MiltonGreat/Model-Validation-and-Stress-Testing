# Credit Risk Model Validation & Stress Testing

A Basel III-Compliant Framework for PD Model Assessment

### Project Overview

This project extends a credit risk model with:

- Rigorous validation (K-fold, stratified, holdout)
- Economic stress testing (PD shocks, feature sensitivity)
- Regulatory-ready reporting (AUC, Brier, tail risk metrics)

Built to audit Internal Ratings-Based (IRB) models under Basel III requirements.

### Dataset

The dataset contains financial and demographic information related to credit applicants. The key features used in this model include:

- Credit History – Previous loan repayment behavior.
- Purpose – The reason for applying for credit.
- Savings – Amount of savings available.
- Amount – Loan amount requested.
- Duration – Loan repayment period.

The target variable is Credit Risk (Good/Bad Credit), where 1 represents bad credit and 0 represents good credit.

### Methodology

The project follows a structured approach to building a credit scorecard:

1. Initialize & Load Data
2. Run Validation Suite
3. Execute Stress Tests
4. Generate Reports

### Insights & Limitations

1. **High Baseline Risk**: 70% default rate suggests non-standard portfolio (verify data).
2. **Economic Sensitivity**: Severe crises disproportionately impact high-risk loans (90th percentile PDs ↑15%).
3. **Loan Size Effect**: Smaller loans (<€5k) have 5-10% higher PDs—consider risk-based pricing.

### Conclusion

While the model performs adequately given the extreme portfolio risk, the high baseline default rate makes this more suitable for stress testing methodology development than real-world deployment without further validation. 

### Source

![German Credit Data from Kaggle](https://www.kaggle.com/datasets/varunchawla30/german-credit-data)
