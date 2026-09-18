# 🧹 Adventure Works — Power Query Data Cleaning

Power Query was used to **clean, transform, and prepare the Adventure Works dataset** before building the Power BI dashboard.

## 🎯 Objective

Prepare clean, consistent, and analysis-ready data for **sales, product, customer, and return analysis**.

## 🔄 Data Cleaning Process

```text
Raw Data
   ↓
Data Profiling
   ↓
Clean & Transform
   ↓
Validate Data
   ↓
Load to Power BI Model
```

## 🛠️ Key Transformations

- **Removed unnecessary columns** to simplify the data model.
- **Renamed columns** for clear and consistent naming.
- **Changed data types** for IDs, dates, quantities, and financial fields.
- **Handled missing values** based on business requirements.
- **Checked duplicates and errors** to improve data quality.
- **Cleaned text fields** using Trim/Clean and value replacement.
- **Transformed date fields** for time-based analysis.
- **Merged related tables** where additional attributes were required.
- **Created required transformation columns** before loading the data.

## 🔍 Data Validation

Before loading the data into Power BI, the following were checked:

- Row counts
- Missing values
- Duplicate records
- Data types
- Key columns
- Date ranges
- Invalid/error values

## 📊 Output

The cleaned dataset was loaded into Power BI and used for:

**Data Modeling → DAX Measures → KPIs → Dashboard → Business Insights**

### 🧠 Skills Demonstrated

**Power Query | Data Cleaning | Data Transformation | Data Validation | ETL | Data Preparation**