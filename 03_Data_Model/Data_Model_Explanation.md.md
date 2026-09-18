# 🏗️ Adventure Works — Data Model

The Adventure Works Power BI project uses a **relational analytical data model** to connect sales, customer, product, date, and return information for interactive analysis.

## 🎯 Objective

Build a clean and efficient model that supports:

- Sales & revenue analysis
- Profitability analysis
- Product performance
- Customer analysis
- Return analysis
- Time-based trends

## 🗂️ Model Structure

```text id="3h6w8k"
                    ┌──────────┐
                    │   Date   │
                    └────┬─────┘
                         │
                         │
┌──────────┐        ┌────▼─────┐        ┌──────────┐
│ Customer │───────►│  Sales   │◄───────│ Product  │
└──────────┘        └────┬─────┘        └──────────┘
                         │
                         │
                    ┌────▼─────┐
                    │ Returns  │
                    └──────────┘
```

> **Note:** The diagram above is a simplified representation. The actual Power BI model contains the project-specific tables and relationships.

## 🔗 Modeling Approach

- Used a **star/snowflake-style analytical model** based on the available dataset.
- Connected fact and dimension tables using appropriate keys.
- Used **one-to-many relationships** where applicable.
- Created a dedicated **Date table** for time-based analysis.
- Maintained consistent key columns and data types.
- Designed the model to support efficient filtering and DAX calculations.

## 📐 Key Tables

| Table | Purpose |
|---|---|
| **Sales** | Transactions, revenue, orders |
| **Product** | Product and category information |
| **Customer** | Customer details |
| **Date** | Time-based analysis |
| **Returns** | Product return analysis |

## 📊 Model Output

The data model provides the foundation for:

**DAX Measures → KPIs → Interactive Dashboard → Business Insights**

### 🧠 Skills Demonstrated

**Data Modeling | Relationships | Star Schema | Fact & Dimension Tables | Power BI | DAX**