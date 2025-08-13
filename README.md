# Financial-Risk-Analysis
Springboard Capstone I
Financial Risk Analysis
Project Overview
This project examines 15,000 anonymized loan records to determine whether borrower attributes — such as credit score, income, employment status, education, debt-to-income (DTI) ratio, and demographics — have a measurable effect on loan amount. The analysis aims to identify which variables truly influence lending decisions and which have negligible impact, supporting fairer and more transparent lending practices.
Dataset Description
Title: Financial Risk Assessment Source: Structured consumer lending dataset (anonymized) Size: 15,000 rows × 20 columns Data Types:  - Numerical: income, credit score, loan amount, debt-to-income ratio, assets  - Categorical: gender, education level, employment status, marital status, loan purpose, risk rating Format: Clean CSV, minimal missing data, mixed variable types
Methodology
1. Data Exploration    - Summary statistics and visualizations for all numerical and categorical features    - Outlier detection and missing value analysis  2. Univariate & Bivariate Analysis    - Compared loan amount distributions across demographic and financial variables    - Boxplots, scatterplots, and grouped summaries  3. Regression Analysis    - Multiple linear regression to model loan amount as a function of key features    - Residual diagnostics to check assumptions and model fit  4. Feature Evaluation    - Measured predictive strength of variables using R² and p-values    - Compared statistical significance with practical relevance  5. Visualization    - Tableau dashboards to communicate findings    - Clear charts showing loan size vs. borrower characteristics
Key Insights & Results
- No significant effect on loan amount from: gender, marital status, employment type, or risk rating - Minimal predictive power from: credit score, education level, income group (influences loan volume but not amount) - Weak but statistically significant correlation for DTI (R² < 0.1%) — practically negligible - Loan purpose showed little variation in loan size, averaging ~$27K–$28K across categories - Lending decisions in this dataset appear largely independent of borrower demographics
How to Run the Project
Requirements: pip install pandas numpy matplotlib seaborn statsmodels jupyter  Steps: 1. Clone the repository:    git clone https://github.com/yourusername/financial-risk-analysis.git    cd financial-risk-analysis 2. Place financial_risk_assessment.csv in the project directory 3. Open the Jupyter Notebook:    jupyter notebook Capstone_FinancialRiskAnalysis.ipynb 4. To view the Tableau dashboard, open the .twbx file in Tableau Public/Desktop
Visualizations
- Loan amount distribution by demographic group - Boxplots for DTI vs. loan amount - Scatterplots for credit score vs. loan size - Tableau dashboards for borrower segmentation and variable impact
Future Improvements
- Build a multivariate regression or ML model to combine attributes for improved prediction - Integrate approval/denial policy data for deeper insight - Enrich dataset with loan term, collateral, and repayment history - Analyze attribute effects within credit score bands
