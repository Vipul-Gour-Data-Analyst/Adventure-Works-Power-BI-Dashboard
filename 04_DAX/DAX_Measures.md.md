# 📐 Adventure Works — DAX Measures

DAX was used in Power BI to create **business KPIs, performance metrics, and analytical calculations** for the Adventure Works dashboard.

## 🎯 Objective

Create reusable measures to analyze:

- Revenue
- Profit
- Orders
- Customers
- Returns
- Profitability
- Sales performance

## 📊 Key Measures

### 💰 Total Revenue

```DAX
Total Revenue =
SUM(Sales[Sales Amount])
```

### 💵 Total Profit

```DAX
Total Profit =
SUM(Sales[Profit])
```

### 🛒 Total Orders

```DAX
Total Orders =
DISTINCTCOUNT(Sales[Order Number])
```

### 👥 Total Customers

```DAX
Total Customers =
DISTINCTCOUNT(Customer[Customer Key])
```

### 🔄 Total Returns

```DAX
Total Returns =
SUM(Returns[Return Quantity])
```

### 📈 Profit Margin

```DAX
Profit Margin =
DIVIDE(
    [Total Profit],
    [Total Revenue],
    0
)
```

### 🔄 Return Rate

```DAX
Return Rate =
DIVIDE(
    [Total Returns],
    [Total Orders],
    0
)
```

## 📅 Time Intelligence

DAX time-intelligence calculations were used where required for:

- Year-to-Date (YTD)
- Previous Year
- Year-over-Year (YoY) Growth
- Monthly trends
- Period comparisons

Example:

```DAX
Revenue LY =
CALCULATE(
    [Total Revenue],
    SAMEPERIODLASTYEAR('Date'[Date])
)
```

```DAX
Revenue YoY % =
DIVIDE(
    [Total Revenue] - [Revenue LY],
    [Revenue LY],
    0
)
```

## 🧠 DAX Concepts Demonstrated

- `SUM`
- `DISTINCTCOUNT`
- `CALCULATE`
- `DIVIDE`
- `SAMEPERIODLASTYEAR`
- Filter Context
- Row Context
- Time Intelligence
- KPI Measures

## 📊 DAX Output

These measures power the dashboard's:

**KPI Cards → Charts → Tables → Trend Analysis → Business Insights**

### 🛠️ Skills Demonstrated

**DAX | Power BI | KPI Development | Time Intelligence | Filter Context | Business Calculations**