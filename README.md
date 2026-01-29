# Megaline Statistical Analysis

## Project Overview
This project analyzes customer behavior and revenue patterns for a telecom company by examining usage data across different mobile plans and regions. The goal is to understand how customers use calls, messages, and internet services, calculate monthly revenue, and determine whether statistically significant differences exist between plans and regions.

---

## Project Access
You can explore the full project, analysis, and code directly in this  
[Notebook](/code/hypothesis_project.ipynb).

All calculations, visualizations, and hypothesis testing steps are documented in the Jupyter Notebook.

---

## Datasets Description
The project is based on multiple datasets representing user information, usage activity, and plan details.

---

## Data Preparation and Validation
Before performing any analysis, the datasets were validated and cleaned:

- Checked data types and performed necessary type casting  
- Verified the presence of duplicated values  
- Checked for missing (null) values  
- Reviewed dataset structure using `.info()`  

---

## Feature Engineering & Aggregation
Monthly usage metrics were calculated for each user:

- Monthly number of calls  
- Total call duration (minutes) per month  
- Monthly message count per user  
- Monthly internet usage per user  
- Converted internet usage from **MB to GB**  
- Calculated monthly averages  

---

## Revenue Calculation
Monthly revenue per user was calculated by:

- Applying plan-specific pricing rules  
- Calculating extra charges for usage beyond plan limits  
- Computing total monthly payment per user  
- Aggregating monthly revenue by plan  

---

## Exploratory Data Analysis (EDA)
The following descriptive statistics and distributions were analyzed:

- Mean, variance, and standard deviation of monthly revenue  
- Distribution of monthly call duration by plan  
- Distribution of monthly message usage by plan  
- Distribution of monthly internet usage by plan  

These analyses helped identify skewness and variability in user behavior.

---

## Hypothesis Testing
To evaluate statistical differences between groups, the following tests were used:

- **Shapiro–Wilk Test** to check normality of distributions  
- **Mann–Whitney U Test** to compare groups due to non-normal distributions  

Hypothesis tests were conducted to answer:
- Do Surf and Ultimate plan users have different average monthly revenues?
- Do users in the NY–NJ region have different average monthly revenues compared to other regions?

---

## Tools & Libraries
- Python  
- pandas  
- numpy  
- scipy.stats  
- matplotlib  
- seaborn  

---

## Conclusion
The analysis provides insights into customer usage patterns, revenue differences across plans, and regional variations. Statistical testing confirms whether observed differences are significant, supporting data-driven business decisions.
