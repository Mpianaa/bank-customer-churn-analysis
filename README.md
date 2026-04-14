# Bank Customer Churn Analysis

## Overview
An Excel dashboard analysing churn behaviour across 10,000 bank customers
across France, Germany and Spain.

## Dashboard Preview

### Overview — KPI Cards & Charts
![Dashboard Overview 1](dashboard_overview_1.png)

### Full Chart View
![Dashboard Overview 2](dashboard_overview_2.png)

## Project Description

This project presents a comprehensive analysis of customer churn behaviour 
for a bank with operations across France, Germany, and Spain. Using a dataset 
of 10,000 customer records, the goal was to identify the key factors that 
drive customers to leave the bank and to segment the customer base by risk level.

The analysis was built entirely in Microsoft Excel, covering data cleaning, 
feature engineering, pivot table analysis, KPI tracking, and interactive 
dashboard visualisation.

The project answers the following business questions:
- What is the overall churn rate and how many customers were lost?
- Which geographic market has the highest churn problem?
- Which age group is most likely to leave the bank?
- Does gender influence churn behaviour?
- Do active members stay longer than inactive ones?
- How do balance, salary and credit score relate to churn?
- What does the profile of a typical churned customer look like?

## Dataset Description
The dataset contains 10,000 rows and 13 original columns:

| Column | Description |
|--------|-------------|
| CustomerId | Unique identifier for each customer |
| Surname | Customer surname |
| CreditScore | Customer credit rating (350–850) |
| Geography | Country — France, Germany or Spain |
| Gender | Male or Female |
| Age | Customer age in years |
| Tenure | Number of years with the bank (0–10) |
| Balance | Current account balance |
| NumOfProducts | Number of bank products held |
| HasCrCard | Whether customer has a credit card (Yes/No) |
| IsActiveMember | Whether customer is an active member (Active/Inactive) |
| EstimatedSalary | Customer's estimated annual salary |
| Exited | Whether the customer churned (Churned/Retained) |

Five additional columns were engineered for segmentation analysis:

| Column | Description |
|--------|-------------|
| Age Group | Grouped age bands (<25, 26-35, 36-45, 46-55, 56-65, Over 65) |
| Salary Band | Salary ranges (<50K, 50K-100K, 100K-150K, 150K+) |
| Balance Band | Balance ranges (Zero, 1-50K, 50K-100K, 100K-150K, 150K+) |
| Credit Score Band | Score ranges (350-500, 501-600, 601-700, 701-800, 801-850) |
| IsChurned | Binary flag (1 = Churned, 0 = Retained) |

## Dashboard Structure

The workbook contains three sheets:

- **Raw Data** — Full cleaned dataset with all original and derived columns
- **Pivot Tables** — Dynamic pivot tables for interactive segment exploration
- **Dashboard Overview** — Visual dashboard with KPI cards and charts


## Key Findings
- Overall churn rate: 20.4% (2,037 customers)
- Germany has the highest churn rate at 32.4%
- Age group 46-55 is highest risk at 50.6% churn
- Customers with 3-4 products have extremely high churn (83-100%)
- Inactive members churn at nearly double the rate of active members


 High Risk Customer Profile Summary
The combination of factors most associated with churn:

Age: 46–55

Geography: Germany

Gender: Female

Membership: Inactive

Products held: 3 or 4

Balance: $100K–$150K

  
1. Overall Churn

Out of 10,000 customers, 2,037 churned — a churn rate of 20.4%
The bank successfully retained 7,963 customers (79.6%)


2. Geography — Germany is the biggest problem

Germany churn rate: 32.4% — nearly double France (16.2%) and Spain (16.7%)
Germany has only 25% of total customers yet accounts for 40% of all churn

3. Age Group — Middle-aged customers are highest risk

46–55 is the most dangerous segment at 50.6% churn — 1 in 2 customers left.
Young customers (Under 25 and 26–35) are the safest at under 9% churn


4. Gender — Females churn significantly more

Female churn rate: 25.1% vs Male: 16.5%
1,139 females churned compared to 898 males despite females being fewer in total


5. Number of Products — Critical red flag

Customers with 3 products: 82.7% churn rate
Customers with 4 products: 100% churn rate — every single one left
Customers with 2 products are the most loyal at just 7.6% churn
Having too many products is actually a strong churn predictor.


6. Active vs Inactive Members

Inactive members churn at 26.9% vs Active members at 14.3%
Engagement is a strong retention signal — active members are nearly twice as likely to stay


7. Balance Band — Mid-to-high balances churn more

1–50K band has the highest churn rate at 34.7%
100K–150K follows at 25.8%
Zero balance customers are actually safer at 13.8% churn


8. Credit Score — Marginal impact

Lower scores (350–500) churn slightly more at 23.6%
Difference across all bands is small — credit score is not a strong churn predictor alone


9. Salary — Almost no impact

All salary bands hover around 19–21% churn
Salary alone does not predict whether a customer will churn

10. Tenure

Customers with 0–1 years tenure churn the most — new customers are highest risk early on
Churn rate gradually decreases from year 2 to year 7 as customers settle in
A slight dip occurs at year 7 suggesting a loyalty plateau
Churn rises again slightly at years 9–10 — long-term customers are not completely safe
Average tenure of churned customers: 4.93 years
Average tenure of retained customers: 5.03 years — almost identical showing tenure alone does not predict loyalty


## Skills Demonstrated
- Data cleaning and preparation in Excel
- Feature engineering using nested IF formulas
- Pivot Tables with custom grouping and slicers
- COUNTIFS, AVERAGEIF, and SUMIF formula logic
- KPI card design and dashboard layout
- Data storytelling and business insight generation
