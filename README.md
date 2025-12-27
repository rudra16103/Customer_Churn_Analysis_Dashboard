<img width="204" height="204" alt="image" src="https://github.com/user-attachments/assets/c140b495-6cac-4ce3-9985-b5c96f8f013b" />


# Customer Churn Analysis Dashboard (Power BI)

## Project Overview
Customer churn is a major business challenge where customers stop using a company’s services.  
This project analyzes **why customers churn** using the **Telco Customer Churn dataset** and presents insights through an **interactive Power BI dashboard**.

The dashboard helps stakeholders understand churn patterns, identify high-risk customer segments, and explore churn drivers using drill-through analysis.

---

## Project Objectives
- Measure overall customer churn and retention
- Identify key drivers contributing to customer churn
- Analyze churn across contract type, tenure, services, and billing methods
- Enable deeper analysis using drill-through pages
- Present insights in a clean, business-friendly dashboard

---

## Tools & Technologies
- **Power BI Desktop**
- **Power Query** – data cleaning and feature engineering
- **DAX** – KPI calculations and business measures
- **Dataset Source** – Kaggle (Telco Customer Churn)

---

## Dataset Information
- **Source:** Telco Customer Churn (Kaggle)
- **Records:** 7,043 customers
- **Target Variable:** Churn (Yes / No)

**Key attributes include:**
- Customer demographics
- Contract and billing details
- Internet and service usage
- Tenure and charges

---

## Data Preparation (Power Query)
The following transformations were performed:
- Promoted headers and corrected data types
- Converted `SeniorCitizen` from 0/1 to Yes/No
- Standardized service-related values (e.g., *No internet service → No*)
- Created derived columns:
  - **Tenure Group** (0–12, 13–24, 25–48, 49+ months)
  - **Monthly Charges Group** (Low / Medium / High)
- Reordered columns for readability

All transformations were kept minimal and purpose-driven.

---

## Key DAX Measures
Key measures used in the dashboard include:
- **Total Customers**
- **Churned Customers**
- **Churn Rate (%)**
- **Average Monthly Charges**
- **Revenue Lost due to Churn**

These measures drive all KPIs, charts, and drill-through analysis.

---

## Dashboard Structure

### 🔹 Main Dashboard (Executive Overview)
- KPI Cards:
  - Churn Rate (%)
  - Total Customers
  - Churned Customers
  - Average Monthly Charges
- Churn Rate by **Contract Type**
- Churn Rate by **Tenure Group**
- **Key Influencers** visual to identify churn drivers
- Interactive slicers for Contract, Tenure Group, Payment Method, and Internet Service

---

### Drill-Through Pages (Detailed Analysis)

#### Contract & Billing Churn Analysis
- Churn Rate by Contract
- Churn Rate by Payment Method
- Revenue Lost
- Detailed customer-level table

#### Service & Customer Profile Analysis
- Churn Rate by Internet Service
- Churn Rate by Tenure Group
- Service-related churn patterns
- Supporting KPIs

Drill-through pages allow deeper analysis without overcrowding the main dashboard.

---

## Key Insights
- Customers on **month-to-month contracts** are over **6× more likely to churn**
- Churn is highest during the **first 12 months** of customer tenure
- **Fiber optic internet users** show significantly higher churn
- Customers using **electronic check** payment methods have higher churn rates
- Long-term contracts greatly improve customer retention

---

## Business Value
This analysis helps businesses:
- Identify high-risk customer segments
- Reduce revenue loss by addressing churn drivers
- Improve retention strategies
- Support data-driven decision-making

---
