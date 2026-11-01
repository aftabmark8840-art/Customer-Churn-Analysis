# Customer Churn Analysis using SQL & Python

A complete end-to-end Customer Churn Analysis project built using **SQLite, SQL, Python (Pandas, NumPy, Matplotlib, Seaborn)**. The project demonstrates how customer, subscription, and support data can be combined to uncover churn trends, customer behavior, revenue impact, and actionable business insights. The analysis includes data cleaning, feature engineering, exploratory data analysis (EDA), correlation analysis, and visualization.

---

## Project Objectives

- Analyze customer churn behavior.
- Calculate business KPIs related to churn and retention.
- Identify high-risk customer segments.
- Analyze churn across subscription plans and states.
- Estimate revenue and impact due to churn.
- Generate actionable business recommendations.

---

## Tech Stack

- Python
- SQLite
- SQL
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Jupyter Notebook

---

## 📂 Dataset

The project uses three relational tables:

### 1. Customer Table
Contains customer demographic information.

- Customer ID
- Customer Name
- Gender
- State
- Country
- Date of Birth

### 2. Subscription Table
Contains subscription and billing details.

- Plan Type
- Contract Type
- Monthly Charges
- Subscription Type
- Renewal Date
- Cancellation Date
- Cancellation Reason
- CLTV
- Churn Score

### 3. Support Table
Contains customer support interactions.

- Complaint Date
- Escalation Status
- CSAT Score
- Complaint Count

The three tables are joined using **Customer ID** for analysis.

---

# Data Cleaning & Feature Engineering

The following preprocessing steps were performed:

- Converted date columns into datetime format.
- Filled missing country values.
- Standardized gender values.
- Removed unnecessary columns.
- Created **Churn Flag** using Cancellation Date.
- Calculated Customer Tenure.
- Generated Complaint Count.
- Created Churn Risk category using Churn Score.


---

# Key Business KPIs

| KPI | Value |
|------|------:|
| Total Customers | 121 |
| Churn Rate | **10.74%** |
| Retention Rate | **89.26%** |
| Average Revenue Per User (ARPU) | **₹525.59** |
| Average Customer Tenure | **1576 Days** |
| Revenue at Risk | **₹4,166.94** |
| Average Complaints per Customer | **0.48** |
| Escalation Rate | **3.31%** |


---

# Exploratory Data Analysis

The project includes analysis of:

- Churn Rate
- Retention Rate
- Churn by Plan Type
- Churn by State
- Customer Distribution
- Revenue Analysis
- Customer Tenure
- Complaint Analysis
- Escalation Analysis
- Correlation Analysis
- Monthly Churn Trend
- Yearly Churn Trend
- Contract-wise Churn
- Subscription Type Analysis


---

# Major Insights

### Overall Business

- Customer retention remains high at **89.26%**.
- Overall churn rate is **10.74%**, indicating relatively stable customer retention.
- Average customer tenure exceeds **4 years**, suggesting long-term customer engagement.

### Plan-wise Insights

- **Basic Plan** has the highest churn rate (**14.29%**).
- Nearly **46% of all churned customers** belong to the Basic Plan.
- Premium customers exhibit the lowest churn.

### Geographic Insights

- Karnataka contributes the largest share of churned customers (**30.77%**).
- Delhi and Meghalaya are the next most affected regions.

### Revenue Insights

- Average monthly revenue per customer (ARPU) is **₹525.59**.
- Total monthly revenue at risk from churned customers is approximately **₹4,166.94**.

### Customer Support Insights

- Average complaints per customer are **0.48**.
- Escalation rate is only **3.31%**, indicating most issues are resolved without escalation.
- Escalation shows a **moderate positive correlation (0.53)** with churn, suggesting unresolved issues increase churn likelihood.

### Contract Insights

- Month-to-month and monthly contracts experience higher churn compared with long-term contracts.
- Annual and longer-term contracts exhibit stronger customer retention.


---

# Visualizations

The notebook contains visualizations including:

- Yearly Churn Trend
- Monthly Churn Trend
- Churn by Plan Type
- Churn by State
- Correlation Heatmap
- Pair Plot
- Multi-dimensional CatPlot
- Pivot Tables


---

# Business Recommendations

- Investigate the high churn observed in **Karnataka** to identify operational or service-related issues.
- Review pricing and feature changes for the **Basic Plan**, as it accounts for the largest share of churn.
- Prioritize customers with **High** and **Medium** churn risk scores for proactive retention campaigns.
- Contact at-risk customers via email, SMS, or phone before renewal.
- Improve customer support response time to minimize escalations.
- Encourage migration from monthly plans to long-term contracts through targeted offers and discounts.
- Continuously monitor complaint trends and customer satisfaction (CSAT) to reduce churn risk.

---

# 📁 Project Structure

```
OTT_Churn_Analysis/
│
├── churn_analysis_aug.ipynb
├── churn_analysis - Copy.pdf
├── exported_churn_aug.csv
├── churn_analysis_aug.db
├── README.md
```

