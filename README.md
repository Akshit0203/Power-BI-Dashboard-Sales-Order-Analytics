# Power BI Sales & Order Analytics Dashboard

<p align="center"> <img src="Screenshots/Dashboard.png" alt="Power BI Sales & Order Analytics Dashboard"> </p>

<p align="center"> <strong>Interactive Business Intelligence Dashboard for Sales, Profitability & Order Performance</strong> </p>

---

## 📌 Project Overview

**Power BI Sales & Order Analytics** is an interactive Business Intelligence dashboard developed to transform transactional sales data into actionable business insights.

The solution provides a consolidated view of **sales, profitability, orders, customers, products, geography, segments, shipping modes, and time-based performance** through interactive visualizations and dynamic filtering.

The project covers the complete BI development lifecycle:

**Data → Transformation → Modeling → DAX → Visualization → Analysis**

---

## 🎯 Business Objectives

The dashboard was developed to provide visibility into key areas of business performance:

- Monitor overall sales and profitability
    
- Track order volume and quantity
    
- Analyze regional and country-level performance
    
- Identify product and sub-category trends
    
- Evaluate customer segment performance
    
- Analyze shipping mode distribution
    
- Identify sales and profit trends over time
    
- Enable interactive exploration through filters and drill-downs
    

---

## 📊 Dashboard

The dashboard combines KPI cards, charts, slicers, and drill-down functionality to provide an interactive analytical experience.
### Key Analytical Dimensions

| Dimension     | Analysis                |
| ------------- | ----------------------- |
| 🌍 Geography  | Region & Country        |
| 📦 Products   | Category & Sub-Category |
| 👥 Customers  | Customer & Segment      |
| 🚚 Operations | Shipping Mode           |
| 📅 Time       | Date & Trends           |
| 💰 Finance    | Sales, Cost & Profit    |

---

## 📈 Key Performance Indicators

The dashboard incorporates custom DAX measures for core business KPIs.

|KPI|Purpose|
|---|---|
|**Total Sales**|Measures overall revenue generated|
|**Total Profit**|Measures total profitability|
|**Profit Margin**|Evaluates profit relative to sales|
|**Order Volume**|Measures unique order activity|
|**Average Sales per Order**|Measures average sales value per order|
|**Total Quantity**|Measures total units ordered|

Detailed DAX calculations are available in:

📄 **[DAX Measures](Documentation/DAX_Measures.md)**

---

## 🔄 Data Preparation & ETL

The source dataset was provided in Microsoft Excel and prepared using **Power Query**.

### Transformation Process

```text
                ┌─────────────────────┐
                │   Excel Dataset     │
                └──────────┬──────────┘
                           │
                           ▼
                ┌─────────────────────┐
                │    Power Query      │
                │ Cleaning & ETL      │
                └──────────┬──────────┘
                           │
                           ▼
                ┌─────────────────────┐
                │    Data Model       │
                └──────────┬──────────┘
                           │
                           ▼
                ┌─────────────────────┐
                │   DAX Measures      │
                └──────────┬──────────┘
                           │
                           ▼
                ┌─────────────────────┐
                │ Power BI Dashboard  │
                └──────────┬──────────┘
                           │
                           ▼
                ┌─────────────────────┐
                │ Business Analysis   │
                └─────────────────────┘
```

### Data Preparation Activities

- Data cleaning and transformation
    
- Data type validation
    
- Dataset structuring
    
- Field preparation
    
- Data integrity checks
    
- Preparation for analytical modeling
    

---

## 🧩 Data Model

The analytical model supports multiple dimensions for interactive reporting.

```text
                    SALES & ORDERS
                         │
        ┌────────────────┼────────────────┐
        │                │                │
        ▼                ▼                ▼
   Geography         Products         Customers
        │                │                │
   ┌────┴────┐      ┌────┴────┐      └── Segment
   │         │      │         │
 Region   Country Category  Sub-Category
        │
        ▼
      Time
        │
       Date

        │
        ▼
    Operations
        │
   Shipping Mode
```

For detailed model documentation:

📄 **[Data Model](Documentation/Data_Model.md)**

---

## 💡 Analytical Capabilities

The dashboard enables users to explore business performance through dynamic filtering and drill-downs.
### Regional Analysis

Compare sales and profitability across regions and countries.
### Product Analysis

Analyze performance across product categories and sub-categories.
### Customer Analysis

Explore customer purchasing behavior and segment-level performance.
### Shipping Analysis

Examine order activity across different shipping modes.
### Time-Series Analysis

Analyze sales and profit trends over time and identify seasonal patterns.

---

## 🖼️ Dataset

The underlying transactional dataset is provided in Excel format.

<p align="center"> <img src="Screenshots/Dataset.png" alt="Dataset Preview"> </p>

### Dataset Fields

```text
Order ID
Date
Customer
Product Category
Region
Segment
Shipping Mode
Cost
Sales
Profit
Quantity
```

---

## 🛠️ Technology Stack

|Technology|Role|
|---|---|
|**Microsoft Power BI**|Dashboard & visualization|
|**Power Query**|Data preparation & ETL|
|**DAX**|Measures & KPI calculations|
|**Microsoft Excel**|Source dataset|
|**Data Modeling**|Analytical data structure|

---

## 📁 Repository Structure

```text
power-bi-sales-order-analytics/
│
├── README.md
│
├── PowerBI/
│   └── Sales_Order_Analytics.pbix
│
├── Dataset/
│   └── Power_BI_Dataset.xlsx
│
├── Screenshots/
│   ├── Dashboard.png
│   └── Dataset.png
│
└── Documentation/
    ├── DAX_Measures.md
    ├── Data_Model.md
    └── Project_Documentation.md
```

---

## 📚 Documentation

|Resource|Description|
|---|---|
|**[Project Documentation](Documentation/Project_Documentation.md)**|Complete project methodology and workflow|
|**[DAX Measures](Documentation/DAX_Measures.md)**|DAX calculations and KPI definitions|
|**[Data Model](Documentation/Data_Model.md)**|Data structure and analytical model|

---

## 🧠 Skills Demonstrated

**Business Intelligence**
**Data Analytics**
**Data Visualization**
**Microsoft Power BI**
**Power Query / ETL**
**DAX**
**Data Modeling**
**KPI Development**
**Interactive Dashboard Development**
**Sales & Order Analytics**
**Business Data Analysis**
**Data Storytelling**

---

## 🚀 Project Outcome

This project demonstrates the ability to take a raw transactional dataset and develop a complete Business Intelligence solution using Microsoft Power BI.

The final solution combines **data preparation, analytical modeling, DAX-based metrics, interactive visualization, and business analysis** into a single reporting environment.

---

## ⭐ If You Find This Project Useful

If this project helped you or you found it interesting, consider giving the repository a ⭐.

---

## 📄 License

This project is intended for **educational and portfolio purposes**.