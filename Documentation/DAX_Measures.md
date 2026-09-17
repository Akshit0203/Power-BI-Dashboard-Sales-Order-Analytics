# DAX Measures

This document contains the key DAX-based metrics used in the Power BI Sales & Order Analytics dashboard.

## 1. Total Sales

Calculates the overall sales generated across the dataset.

```DAX
Total Sales =
SUM('Data'[Sales])
```

---

## 2. Total Profit

Calculates the total profit generated across all orders.

```DAX
Total Profit =
SUM('Data'[Profit])
```

---

## 3. Profit Margin

Calculates profitability as a percentage of total sales.

```DAX
Profit Margin =
DIVIDE(
    [Total Profit],
    [Total Sales],
    0
)
```

Format this measure as a **percentage** in Power BI.

---

## 4. Order Volume

Calculates the number of orders in the dataset.

```DAX
Order Volume =
DISTINCTCOUNT('Data'[Order ID])
```

Using `DISTINCTCOUNT` ensures that an order is counted once even if the dataset contains multiple rows associated with the same order.

---

## 5. Average Sales per Order

Calculates the average sales generated per order.

```DAX
Average Sales per Order =
DIVIDE(
    [Total Sales],
    [Order Volume],
    0
)
```

---

## 6. Quantity

Calculates the total quantity associated with the orders.

```DAX
Total Quantity =
SUM('Data'[Quantity])
```

---

## 7. Time-Based Analysis

Time-based calculations can be used to analyze changes in sales and profit over time.

Examples include:

- Sales trends by date
    
- Monthly sales performance
    
- Yearly sales performance
    
- Profit trends
    
- Period-over-period comparisons
    

The dashboard uses date-based analysis to support trend identification and seasonal analysis.

---

## 8. Dynamic Filtering

The DAX measures are designed to respond dynamically to Power BI filter context.

For example, applying a filter for a specific:

- Region
    
- Country
    
- Segment
    
- Category
    
- Sub-Category
    
- Shipping Mode
    

will dynamically recalculate the relevant KPI values.

This allows the same measures to be used across multiple dashboard visuals while maintaining interactive analysis.

---

## 9. DAX Design Principles

The measures follow several core principles:

- Reusable measures instead of unnecessary repeated calculations
    
- `DIVIDE()` for safe division
    
- Filter-context-aware calculations
    
- Distinct order counting where appropriate
    
- Measures designed for interactive dashboard analysis
    

> **Note:** The table name `Data` used in the examples should be replaced with the actual table name in the Power BI model if it differs.