# Loan Default Risk Analysis

This repository contains the code, data, and results of an exploratory data analysis (EDA) project aimed at understanding the factors driving loan defaults in a lending portfolio.

## Business Objective

The primary objective of this project is to identify key drivers of loan default risk. This knowledge will enable the bank to:

* **Improve risk assessment:** Develop more accurate risk scoring models to identify high-risk applicants.
* **Refine loan approval criteria:** Adjust lending policies to minimize risk and improve portfolio quality.
* **Implement targeted risk management strategies:** Develop specific strategies for managing risk within different client segments.
* **Enhance decision-making:** Make more informed decisions regarding loan approvals, pricing, and risk mitigation.

## Data

* **Data Sources:**
    * Application Data: Information about the client's loan application.
    * Previous Application Data: Information about clients' previous loan applications.

* **Data Cleaning and Preprocessing:**
    * Performed proper Data cleaning steps including handling missing values, outlier detection, etc.

## Methodology

1. **Univariate Analysis:**
    * Analyzed the distribution of key variables (e.g., loan amount, income, age, employment duration) and identified potential outliers or unusual patterns.
    * Identified segments with potentially higher default risk.

2. **Bivariate Analysis:**
    * Explored the relationship between individual variables and the target variable (`TARGET`).
    * Identified key predictors of default risk, including:
        * **Strong Predictors:** `EXT_SOURCE_2`, `EXT_SOURCE_3`
        * **Potential Risk Factors:** Larger loan amounts, clients with Cash loans, Refused or Canceled previous applications, clients with lower education levels, certain income types (e.g., "Working"), clients who do not own a car or a house.

3. **Multivariate Analysis:**
    * **Pairplot Analysis:** Visualized the relationships between key variables and the target variable. Observed potential interactions between variables (e.g., loan amount, annuity payment, and external scores).
    * **Correlation Analysis:** 
        * Identified strong correlations between `EXT_SOURCE_2`, `EXT_SOURCE_3`, and the target variable.
        * Observed correlations between loan amount, annuity payment, income, and default risk.
        * Analyzed the impact of regional factors, income type, and previous application history on default risk.

## Key Findings

* **Strong Predictors:** `EXT_SOURCE_2` and `EXT_SOURCE_3` emerged as strong predictors of default risk.
* **Loan Characteristics:** Higher loan amounts and annuity payments are associated with increased risk.
* **Client Demographics:** Clients with certain income types (e.g., "Working"), lower education levels, and specific gender (e.g., male) might have higher default risk.
* **Regional Factors:** Regional factors play a significant role in default risk, with some regions exhibiting higher default rates than others.
* **Previous Application History:** Clients with a history of refused or canceled applications have a higher risk of default.

## Recommendations

* **Prioritize risk assessment:** Implement robust scoring systems that incorporate `EXT_SOURCE_2` and `EXT_SOURCE_3` as key risk indicators.
* **Refine loan approval criteria:** Adjust loan approval criteria based on risk factors identified (e.g., loan amount, annuity payment, client characteristics).
* **Targeted risk management:** Develop targeted risk management strategies for high-risk segments (e.g., clients with lower external scores, higher loan amounts, certain income types).
* **Continuous monitoring:** Continuously monitor and refine risk assessment models to adapt to changing market conditions and client behavior.
* **Further research:** Explore the use of advanced machine learning models, investigate the impact of macroeconomic factors, and leverage alternative data sources to enhance risk prediction.

## Tools and Technologies

* **Programming Languages:** Python (with libraries like pandas, NumPy, matplotlib, seaborn)
* **Data Visualization:** Matplotlib, Seaborn

## Conclusion

This analysis provides valuable insights into the factors influencing loan default risk. By leveraging these insights, the bank can make more informed lending decisions, reduce loan defaults, and improve overall portfolio performance.
