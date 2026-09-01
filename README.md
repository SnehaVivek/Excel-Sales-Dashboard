# Sales Performance Dashboard | Excel & Power Query

<p align="center">
  <strong>End-to-End Sales Data Cleaning, Analysis & Visualization</strong>
</p>

## Overview

This project demonstrates an end-to-end **sales data analytics workflow in Microsoft Excel**, starting with raw transactional data and transforming it into a structured dataset, analytical summaries, and an interactive sales dashboard.

The project was designed to answer key business questions around **revenue, units sold, regional performance, product categories, and sales trends**.

### Workflow

**Raw Data → Data Cleaning → Data Transformation → Pivot Analysis → Visualization → Business Insights**

---

## Business Objective

The objective of the project was to transform raw sales records into a reliable analytical dataset and develop a dashboard that enables users to:

- Evaluate overall sales performance
- Compare revenue across regions
- Analyze product category performance
- Examine units sold across regions
- Identify sales trends over time
- Compare salesperson performance
- Interactively filter and explore the results

---

## Data Preparation

The raw sales dataset was processed using **Power Query** before analysis.

### Data Cleaning & Transformation

The following steps were performed:

- Imported the raw sales table into Power Query
- Reviewed and corrected column data types
- Standardized date formatting
- Removed unnecessary leading and trailing spaces
- Corrected inconsistent spacing within text fields
- Standardized text values across:
  - Region
  - Salesperson
  - Product Category
- Verified numerical fields such as Units and Revenue
- Validated the cleaned dataset for consistency
- Loaded the transformed data into Excel as `Clean_Sales_Data`

The resulting dataset was structured for reliable downstream analysis.

---

## Dataset Structure

The cleaned dataset contains the following fields:

| Field | Description |
|---|---|
| **Order ID** | Unique identifier for each transaction |
| **Date** | Transaction date |
| **Region** | Geographic sales region |
| **Salesperson** | Sales representative responsible for the transaction |
| **Product Category** | Category of product sold |
| **Units** | Number of units sold |
| **Revenue** | Revenue generated from the transaction |

### Key Dimensions

**Regions:** North, South, East, West

**Product Categories:** Electronics, Furniture, Office Supplies

---

## Analytical Approach

Once the data was cleaned, **Pivot Tables** were used to aggregate and analyze the dataset.

The analysis focused on:

- Revenue by Region
- Revenue by Product Category
- Units Sold by Region
- Monthly Revenue Trends
- Salesperson Performance
- Product Category Contribution
- Regional Sales Performance

These summaries were then connected to **Pivot Charts and Slicers** to create an interactive dashboard.

---

## Dashboard

The final `Student_Dashboard` converts the analysis into a visual reporting interface.

### Dashboard Components

- **Revenue by Region**
- **Units Sold by Region**
- **Revenue by Product Category**
- **Revenue Trend Over Time**
- **Product Category Contribution**
- **Salesperson Performance**
- **Interactive Region Filter**
- **Interactive Product Category Filter**

The dashboard enables users to move from high-level performance metrics to more specific regional and category-level analysis.

---

## Workbook Architecture

The workbook follows a structured analytical workflow:

```text
Raw_Data
    │
    ▼
Power Query
    │
    ├── Data Type Validation
    ├── Text Standardization
    ├── Space Cleaning
    └── Data Transformation
    │
    ▼
Clean_Sales_Data
    │
    ▼
Analysis_Pivot_Table
    │
    ├── Revenue Analysis
    ├── Units Analysis
    ├── Regional Analysis
    └── Category Analysis
    │
    ▼
Student_Dashboard
    │
    └── Charts + Slicers + Visual Insights
