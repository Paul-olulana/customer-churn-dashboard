# 📊 Customer Churn Analysis Dashboard

---

## 📌 Table of Contents

- [Problem Statement](#problem-statement)
- [Datasource](#datasource)
- [Data Preparation](#data-preparation)
- [Data Modeling](#data-modeling)
- [Data Analysis (DAX)](#data-analysis-dax)
- [Data Visualization (Dashboard)](#data-visualization-dashboard)
- [Insights](#insights)
- [Recommendation](#recommendation)
- [How to Use](#how-to-use)
- [Connect](#connect)

---

## 🟠 Problem Statement

This project analyzes **customer churn** for a fictional telecom company.  
The goal is to uncover:
- Which customers are most likely to churn,
- Which services and contract types have the highest churn risk,
- And what actions the company can take to **reduce churn and revenue loss**.

---

## 📁 Datasource

The dataset is a typical churn dataset containing:
- Customer demographics (gender, senior citizen, dependents, partner)
- Account details (contract type, payment method, tenure)
- Services used (Internet Service, Tech Support, Streaming, etc.)
- Monthly & total charges
- Churn flag

---

## 🧹 Data Preparation

Data was first explored and cleaned in **Excel**, then imported into **Power BI**.  
Key steps:
- Checked for null values and corrected data types.
- Created calculated flags (e.g., `Churn_Flag`, `Senior_Citizen_Flag`).
- Added tenure groupings for clearer analysis.

---

## 🗂️ Data Modeling

A **star schema** was created:
- **Fact Table:** `Fact_Churn` — holds measures like churn flag, charges, tenure.
- **Dimension Tables:** `Dim_Customer`, `Dim_Contract`, `Dim_Payment`, `Dim_TenureGroup`, `Dim_Services`.

Relationships were defined to keep the model clean and performant.

---

## 📈 Data Analysis (DAX)

Key DAX measures created:
- `Total Customers`
- `Churned Customers`
- `Churn Rate`
- `Retention Rate`
- `Revenue Lost`
- `Average Monthly Charges`
- Segmented churn rates by tenure, contract, and customer category (senior citizens, partners, dependents).

---

## 📊 Data Visualization (Dashboard)

The report contains **3 interactive pages**:
1. **Customer Churn Dashboard:** KPIs, churn breakdown by gender, tenure group, payment method.
   ![image](https://github.com/user-attachments/assets/358e5553-36dd-4595-b240-f21456c8c964)


2. **Customer Risk Dashboard:** Highlights churn by Internet Service, Tech/Admin Support, Contract & Tenure.
   ![image](https://github.com/user-attachments/assets/c2d63e85-2a56-4fc3-9e50-d4e1b5a5a8f2)

3. **Services Dashboard:** Shows churn breakdown by services used — Streaming, Tech Support, Multiple Lines, etc.
   ![image](https://github.com/user-attachments/assets/540c45c8-e21c-411e-8ad2-31842f60130f)


Navigation buttons and reset filters ensure a smooth user experience.

---

## 💡 Insights

- 📉 Customers with **month-to-month contracts** and **low tenure** churn significantly more.
- 🛠️ Lack of **Tech Support** strongly correlates with higher churn.
- 💰 High-value customers using **Fiber Optic Internet** contribute the most to revenue loss when they churn.
- 📊 Churn is higher among customers without dependents or partners.

---

## ✅ Recommendation

- Offer loyalty perks and discounts for customers in their first 12 months.
- Bundle Tech Support with plans by default.
- Target high-value Internet Service customers with proactive retention offers.
- Focus retention marketing on month-to-month subscribers.

---

## 🚀 How to Use

1. Download the `.pbix` file.
2. Open with **Power BI Desktop**.
3. Interact with slicers, buttons, and explore the dashboard insights.

---

## 📫 Connect

**Created by:** Paul Olulana  
[LinkedIn](https://www.linkedin.com/in/oluwafemi-paul-3a7272265/) | [Portfolio](#) | [Email](mailto:paulolulana00@gmail.com)
