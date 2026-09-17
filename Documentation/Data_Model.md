# Data Model

## Overview

The Power BI Sales & Order Analytics project uses a structured data model to support interactive analysis of sales, orders, customers, products, regions, segments, and shipping modes.

The model was prepared after cleaning and transforming the raw Excel dataset using Power Query.

## Source Dataset

The source data is provided as an Excel workbook containing business transaction information.

Key fields include:

|Field|Description|
|---|---|
|Order ID|Unique identifier for an order|
|Date|Order or transaction date|
|Customer|Customer associated with the order|
|Product Category|Category of the purchased product|
|Region|Geographic region|
|Segment|Customer/business segment|
|Shipping Mode|Shipping method used|
|Cost|Cost associated with the order|
|Sales|Sales amount|
|Profit|Profit generated|
|Quantity|Quantity ordered|

## Data Preparation

The raw Excel data was processed using Power Query before being loaded into the Power BI model.

The preparation process included:

1. Importing the Excel dataset
    
2. Cleaning the source data
    
3. Transforming the data structure
    
4. Validating data types
    
5. Preparing fields for analysis
    
6. Loading the transformed data into Power BI
    

## Analytical Dimensions

The dashboard supports analysis across several dimensions:

```text
Geography
├── Region
└── Country

Products
├── Category
└── Sub-Category

Customers
└── Segment

Operations
└── Shipping Mode

Time
└── Date
```

These dimensions allow users to analyze business performance from different perspectives.

## Measures

The data model supports the primary analytical measures used throughout the dashboard:

- Total Sales
    
- Total Profit
    
- Profit Margin
    
- Order Volume
    
- Average Sales per Order
    
- Total Quantity
    

The detailed DAX definitions are documented in:

`DAX_Measures.md`

## Filter Context

Power BI's filter context allows the measures to dynamically respond to user selections.

For example, selecting a specific region can dynamically update:

- Total Sales
    
- Total Profit
    
- Profit Margin
    
- Order Volume
    
- Average Sales per Order
    
- Quantity
    

The same behavior applies to other dashboard dimensions such as country, segment, category, sub-category, and shipping mode.

## Model Design Goals

The data model was designed with the following goals:

- Maintain data integrity
    
- Support interactive filtering
    
- Enable drill-down analysis
    
- Provide reusable analytical measures
    
- Support time-based analysis
    
- Enable efficient business reporting
    

## Analytical Flow

```text
Raw Excel Dataset
        ↓
Power Query
        ↓
Cleaned & Transformed Data
        ↓
Power BI Data Model
        ↓
DAX Measures
        ↓
Interactive Dashboard
        ↓
Business Insights
```

## Note

This documentation describes the analytical structure and fields supported by the project. Exact table and relationship names should reflect the final Power BI model.