# Summary Report

## Background

This document presents an exploratory analysis of Geldium’s dataset, aimed at evaluating data integrity, uncovering valuable insights, and identifying factors that contribute to the risk of credit default. The primary objective is to prepare the data for accurate predictive modeling and risk evaluation.

## Dataset Summary

This dataset includes 500 customer records from Geldium, each containing essential features related to credit delinquency. It comprises both numerical and categorical data, such as earnings, credit usage, number of missed installments, and the ratio of debt to income.
Important details:
- Total entries: 500
- Major attributes: Age, Income, Credit Score, Credit Utilization, Missed Payments, Debt-to-Income Ratio
- Data types:
    - Categorical: Employment Status, Credit Card Type
    - Numerical: Income, Loan Balance

## Missing Data Evaluation

There are missing entries in crucial variables, especially in the income and loan balance fields. If left untreated, these gaps could distort model accuracy.
Observations:
Fields with missing data:
Income: 50 missing entries
Loan Balance: 30 missing entries

Planned solutions:
- Use the median to fill missing numeric values
- Apply AI-generated synthetic data where appropriate for Loan Balance
- 
## Key Insights and Risk Factors

The analysis indicates a strong link between high credit utilization and delinquency, as well as a clear risk associated with frequent missed payments.
Important insights:

- Customers using more than 50% of their credit limit tend to be at greater risk.
- Individuals with 3 or more missed payments within six months show a higher likelihood of defaulting.
- Some inconsistencies were observed: high-income customers with low credit scores warrant further examination.

### Role of AI & GenAI
Generative AI tools supported the identification of trends, detection of missing values, and examination of risk elements. These AI-based conclusions were compared against established financial risk metrics for validation.
Sample AI queries:

"Summarize data trends and highlight missing values."
"Assess risk of default based on credit usage and payment behavior."

## Conclusion & Future Actions
This EDA uncovered meaningful insights into Geldium’s dataset, highlighting missing entries, behavioral patterns tied to credit risk, and some outlier cases worth deeper analysis.
### Takeaways:

- Data gaps: Missing income and loan data could influence outcomes.
- Delinquency indicators: High credit usage and repeated missed payments are strong predictors.
- Data anomalies: Cases of high income but low credit scores need clarification.

### Recommendations:

- Choose suitable imputation techniques for missing income and loan values to minimize bias.
- Confirm if key risk factors remain consistent across various customer groups.
- Investigate irregular data entries to ensure accuracy and detect potential financial instability.
- These efforts will aid Geldium in refining its risk analysis processes and enhance data reliability for further modeling.

## Summary of Predictive Insights

Based on the EDA and the predictive modeling plan (Task 2), the following insights were observed:

- Customers under 30 years old with two or more missed payments and credit utilization above 50% show significantly higher risk of delinquency.
- High debt-to-income ratio (> 0.5) consistently correlates with late or missed payments.
- Customers with short account tenure (< 12 months) tend to have weaker repayment behavior.

Key Insights Summary Table:

|Key Insight	| Customer Segment| Influencing Variables	| Potential Impact|
|---------|----------|--------|---------|
|Customers with high credit utilization and frequent missed payments are at highest risk of delinquency.	| Under 30 years old, 2+ missed payments, high credit utilization (> 50%)	| Missed Payments, Credit Utilization, Age, Debt-to-Income Ratio | Targeted outreach could reduce 30-day delinquency rates by over 10% in this segment.|

### Recommendation Framework

- Restated Insight:

Customers under 30 with 2+ missed payments and credit utilization above 50% are at significantly high risk of delinquency.

- Proposed Recommendation:

Launch a 6-week SMS outreach campaign targeting these customers to reduce 30-day delinquency by at least 10%.

-Specific:

Target customers under 30 with 2+ missed payments and high credit utilization.

- Measurable:

Track reduction in 30-day delinquency; goal is a 10% decrease.

- Actionable:

Use existing SMS infrastructure for outreach.

