# 🚴 Adventure Works Sales & Performance Dashboard | Power BI

An interactive **Power BI Sales & Performance Dashboard** built using the **Adventure Works dataset** to analyze sales, revenue, profitability, customers, products, orders, and return performance.

The project follows a complete **Data Analyst workflow** — from understanding the business problem and preparing the data to building the data model, creating DAX measures, developing dashboards, and generating business insights.

---

## 📌 Project Overview

**Adventure Works** is a fictional bicycle and accessories company with sales across different products, customers, regions, and sales channels.

The objective of this project is to transform raw sales data into an interactive Power BI dashboard that helps stakeholders understand:

- Sales and revenue performance
- Profitability
- Product performance
- Customer behavior
- Regional performance
- Order trends
- Return performance

---

## 🎯 Business Objectives

The dashboard was developed to answer key business questions such as:

- How are sales and revenue performing over time?
- Which products generate the highest revenue and profit?
- Which regions contribute the most to overall sales?
- Which customers generate the highest revenue?
- What is the overall return rate?
- Which products have higher return rates?
- How do sales and profit change across different periods?
- What areas require further business attention?

---

## 🛠️ Tools & Technologies

| Tool | Purpose |
|---|---|
| **Power BI** | Dashboard development & visualization |
| **Power Query** | Data cleaning & transformation |
| **DAX** | Measures, KPIs & calculations |
| **Excel** | Data source / data preparation |
| **Data Modeling** | Relationships & analytical model |

---

# 📂 Project Structure

```text
Adventure-Works-PowerBI-Project/
│
├── Data/
│   ├── Raw_Data.xlsx
│   └── Data_Dictionary.xlsx
│
├── Power_Query/
│   └── Data_Cleaning_Notes.md
│
├── Data_Model/
│   ├── Data_Model.png
│   └── Data_Model_Explanation.md
│
├── DAX/
│   └── DAX_Measures.md
│
├── Dashboard/
│   ├── Adventure_Works_Sales_Dashboard.pbix
│   └── Screenshots/
│       ├── Executive_Summary.png
│       ├── Sales_Analysis.png
│       ├── Product_Analysis.png
│       ├── Customer_Analysis.png
│       └── Returns_Analysis.png
│
├── Project_Documentation/
│   ├── Project_Report.pdf
│   └── Project_Presentation.pptx
│
├── README.md

```

---

# 🔄 Data Analyst Workflow

```text
Business Problem
       ↓
Business Requirements
       ↓
Data Collection
       ↓
Data Cleaning & Transformation
       ↓
Data Modeling
       ↓
DAX Calculations
       ↓
Dashboard Development
       ↓
Data Analysis
       ↓
Business Insights
       ↓
Documentation
```

---

# 🧹 Data Cleaning & Transformation

The raw dataset was prepared using **Power Query** before building the dashboard.

Key activities included:

- Removing unnecessary columns
- Handling missing values
- Correcting data types
- Cleaning text fields
- Creating required calculated fields
- Standardizing categorical values
- Preparing date-related fields
- Checking data consistency
- Structuring tables for analysis

---

# 🏗️ Data Model

The project uses a structured analytical data model with relationships between sales, customer, product, date, and other supporting tables.

### Main analytical areas

```text
                 Date
                  │
                  │
Customer ───── Sales ───── Product
                  │
                  │
              Returns
```

The model was designed to support interactive filtering and analysis across different business dimensions.

<img width="1320" height="747" alt="AdventureWorks Schema" src="https://github.com/user-attachments/assets/9cb0d03e-ae07-41f2-a503-f3c756ffa2b8" />


---

# 📐 DAX & Measures

DAX was used to create business KPIs and analytical measures.

Example measures include:

```DAX
Total Revenue =
SUM(Sales[Revenue])
```

```DAX
Total Profit =
SUM(Sales[Profit])
```

```DAX
Total Orders =
DISTINCTCOUNT(Sales[OrderNumber])
```

```DAX
Return Rate =
DIVIDE([Total Returns], [Total Orders])
```

Other calculations were created for:

- Revenue
- Profit
- Orders
- Returns
- Average Order Value
- Year-over-Year Growth
- Product performance
- Customer performance
- Regional analysis

---

# 📊 Dashboard Pages

## 1. Executive Summary

Provides a high-level overview of business performance.

### Key KPIs

- 💰 Revenue
- 📈 Profit
- 🛒 Orders
- 👥 Customers
- 🔄 Return Rate

### Dashboard View

<img width="1306" height="750" alt="AdventureWorks Executive View" src="https://github.com/user-attachments/assets/75f69a3b-0086-45fd-9944-543adfc24a52" />

---

## 2. Product Analysis

This page evaluates product-level performance.

### Analysis includes

- Top-performing products
- Revenue by product
- Profit by product
- Product category performance
- Product contribution
- Return performance

<img width="1308" height="750" alt="AdventureWorks Product View" src="https://github.com/user-attachments/assets/96f8cebc-3480-4761-a859-14c33af9ad85" />



---

## 3. Customer Analysis

This page focuses on customer and sales behavior.

### Analysis includes

- Top customers
- Customer revenue contribution
- Customer order trends
- Customer segmentation
- Regional customer performance

<img width="1316" height="750" alt="AdventureWorks Customer View" src="https://github.com/user-attachments/assets/96033a69-2bd2-46c1-8d46-e9695380685a" />



---

# 🔍 Key Business Insights

The dashboard helps identify patterns and trends across sales, profitability, customers, products, and returns.

### Example insights

- Identified the products contributing significantly to overall revenue.
- Analyzed regional differences in sales and profitability.
- Identified high-performing and underperforming products.
- Compared revenue and profit trends over time.
- Analyzed customer contribution to overall sales.
- Identified products and categories with higher return rates.
- Used interactive filtering to investigate business performance at different levels.

> 📌 Replace these examples with your **final validated insights from the dashboard**.

---

# 💡 Business Recommendations

Based on the analysis, stakeholders can use the dashboard to:

- Focus on high-performing products and categories.
- Investigate products with consistently high return rates.
- Monitor regional sales and profitability.
- Identify valuable customer segments.
- Track changes in revenue and profit over time.
- Use product-level insights to support inventory and sales planning.
- Monitor KPIs regularly through the interactive dashboard.

---

# 📸 Dashboard Preview

### Executive Summary

<img width="1306" height="750" alt="AdventureWorks Executive View" src="https://github.com/user-attachments/assets/75f69a3b-0086-45fd-9944-543adfc24a52" />


### Product Analysis

<img width="1308" height="750" alt="AdventureWorks Product View" src="https://github.com/user-attachments/assets/96f8cebc-3480-4761-a859-14c33af9ad85" />


### Customer Analysis

<img width="1316" height="750" alt="AdventureWorks Customer View" src="https://github.com/user-attachments/assets/96033a69-2bd2-46c1-8d46-e9695380685a" />


---

# 📁 Project Files

| File / Folder | Description |
|---|---|
| `Data/` | Raw data and supporting files |
| `Power_Query/` | Data cleaning and transformation documentation |
| `Data_Model/` | Data model and relationship documentation |
| `DAX/` | DAX measures and calculations |
| `Dashboard/` | Power BI dashboard and screenshots |
| `Project_Documentation/` | Detailed project report and presentation |

---

# 🎓 Skills Demonstrated

Through this project, I demonstrated practical skills in:

- Data Cleaning
- Data Transformation
- Power Query
- Data Modeling
- DAX
- KPI Development
- Data Visualization
- Business Analysis
- Sales Analysis
- Profitability Analysis
- Customer Analysis
- Product Analysis
- Return Analysis
- Business Insight Generation
- Dashboard Development

---

# 🚀 Project Outcome

This project demonstrates how a Data Analyst can transform raw business data into an **interactive, business-focused Power BI solution**.

The focus was not only on creating visualizations, but also on understanding the business problem, preparing reliable data, creating meaningful KPIs, analyzing trends, and translating findings into actionable business insights.

---

# 👤 Author

**Vipul Gour**  
Data Analyst | SQL | Power BI | Python | Excel

### Connect With Me

- 💼 **LinkedIn:** https://shorturl.at/bsY3X
- 🌐 **Portfolio:** https://shorturl.at/LfFQg
- 🐙 **GitHub:** https://shorturl.at/DuQdt

---

# ⭐ If You Find This Project Useful

If you found this project helpful or interesting, feel free to **⭐ star this repository** and connect with me on LinkedIn.

Thank you for visiting! 🚀
