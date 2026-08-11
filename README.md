# Databel Customer Churn Analysis

## Overview
This repository contains a comprehensive Power BI analysis on the Databel customer dataset to evaluate customer churn trends, driver categories, and demographic behavioral patterns.

##Dashboard overview
<img width="1178" height="736" alt="Screenshot 2026-08-11 144209" src="https://github.com/user-attachments/assets/72e162cb-4207-4a83-8b6b-d425301356fc" />



## Key Insights & Metrics
* **Total Customers:** 6,687
* **Churned Customers:** 1,796
* **Overall Churn Rate:** 26.86%[cite: 1]
* **Total Charges:** $7M[cite: 1]
* **Average Customer Age:** 47 years[cite: 1]

### Primary Churn Drivers
1. **Competitors:** Accounts for 805 churned customers (primarily due to better offers and superior devices)[cite: 1].
2. **Attitude:** Support person attitude accounts for 287 churned customers[cite: 1].
3. **Dissatisfaction & Price:** Product dissatisfaction (286) and high pricing (200) round out the top primary drivers[cite: 1].

### Key Behavioral Trends
* **Customer Service Calls:** Churn rate dramatically increases when service calls reach 4 or more (jumping from ~36% at 3 calls to over 99% at 4+ calls)[cite: 1].
* **Contract Type:** Monthly contract holders experience a 45–47% churn rate compared to only ~6–7% for yearly contract holders[cite: 1].

---

## DAX Measures & Code

### 1. Total Customers
```dax
Total Customers = COUNT(Databel[Customer ID])
