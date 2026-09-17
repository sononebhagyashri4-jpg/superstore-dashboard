# superstore-dashboard
superstore retail data analysis 
# 📊 Excel Interactive Dashboard

## 📌 Project Overview

This project is an **interactive Excel Dashboard** developed to transform raw data into meaningful business insights.

The dashboard uses **Power Query, Power Pivot, DAX, Pivot Tables, Pivot Charts, Slicers, and Filters** to perform data cleaning, data modeling, analysis, and visualization.

The goal of this project is to demonstrate an end-to-end **data analytics workflow in Microsoft Excel**, from raw data preparation to interactive business reporting.

---

## 🎯 Project Objectives

The main objectives of this project are:

* Clean and transform raw data using **Power Query**.
* Build a structured data model using **Power Pivot**.
* Create dynamic business metrics using **DAX**.
* Analyze data using **Pivot Tables and Pivot Charts**.
* Build an interactive dashboard using **Slicers and Filters**.
* Identify important trends, patterns, and performance indicators.
* Present business insights in a simple and user-friendly format.
* Develop practical skills in Excel-based data analytics and business intelligence.

---

## ❓ Business Questions

The dashboard was designed to answer questions such as:

1. What is the overall business performance?
2. What are the key performance indicators (KPIs)?
3. How does performance change over time?
4. Which products/categories are performing the best?
5. Which regions or segments contribute the most to overall performance?
6. Which areas are underperforming?
7. What are the monthly and yearly trends?
8. Which products or customers generate the highest sales/profit?
9. How does performance change when different filters are applied?
10. What actionable insights can be derived from the data?

---

# 🔄 Project Workflow

The project follows an end-to-end data analytics workflow:

```text
                Raw Data
                    │
                    ▼
             ┌─────────────┐
             │ Power Query │
             └──────┬──────┘
                    │
                    ▼
          Data Cleaning & Transformation
                    │
                    ▼
             ┌─────────────┐
             │ Power Pivot │
             └──────┬──────┘
                    │
                    ▼
              Data Modeling
                    │
                    ▼
             ┌─────────────┐
             │     DAX     │
             └──────┬──────┘
                    │
                    ▼
             DAX Measures
                    │
                    ▼
       Pivot Tables & Pivot Charts
                    │
                    ▼
          Slicers & Interactive Filters
                    │
                    ▼
           📊 Excel Dashboard
                    │
                    ▼
             Business Insights
```

---

# 🗃️ Data

The raw dataset was imported into Excel and prepared for analysis using **Power Query**.

## Data Preparation

Power Query was used for:

* Removing duplicate records
* Handling missing values
* Cleaning inconsistent data
* Changing data types
* Renaming columns
* Formatting dates and numerical fields
* Creating calculated/transformed columns
* Filtering unnecessary records
* Preparing clean tables for the data model

The transformed data was then loaded into **Power Pivot**.

---

# 🧩 Data Model

The cleaned datasets were connected using **Power Pivot** to create a relational data model.

A typical structure of the model is:

```text
                 ┌─────────────────┐
                 │   Date Table    │
                 └────────┬────────┘
                          │
                          │
            ┌─────────────┼─────────────┐
            │             │             │
            ▼             ▼             ▼
     Product Table   Customer Table   Region Table
            │             │             │
            └─────────────┼─────────────┘
                          │
                          ▼
                  ┌──────────────┐
                  │  Fact Table  │
                  │ Transactions │
                  └──────┬───────┘
                         │
                         ▼
                  ┌──────────────┐
                  │ DAX Measures │
                  └──────┬───────┘
                         │
                         ▼
                     Dashboard
```

## Data Modeling Features

* Fact and dimension tables
* Relationships between tables
* Date table for time-based analysis
* One-to-many relationships
* Centralized DAX measures
* Power Pivot data model for efficient analysis

> The exact tables and relationships depend on the dataset used in the project.

---

# 🧮 DAX Measures

**DAX (Data Analysis Expressions)** was used to create dynamic KPIs and analytical measures.

Some example measures include:

### Total Sales

```DAX
Total Sales =
SUM(Sales[SalesAmount])
```

### Total Profit

```DAX
Total Profit =
SUM(Sales[Profit])
```

### Total Orders

```DAX
Total Orders =
DISTINCTCOUNT(Sales[OrderID])
```

### Total Quantity

```DAX
Total Quantity =
SUM(Sales[Quantity])
```

### Average Order Value

```DAX
Average Order Value =
DIVIDE(
    [Total Sales],
    [Total Orders],
    0
)
```

### Profit Margin

```DAX
Profit Margin % =
DIVIDE(
    [Total Profit],
    [Total Sales],
    0
)
```

### Year-to-Date Sales

```DAX
Sales YTD =
TOTALYTD(
    [Total Sales],
    'Date'[Date]
)
```

> **Note:** The DAX formulas above are examples. Replace the table and column names with the actual names used in the workbook.

---

# 📊 Dashboard Features

The dashboard provides an interactive view of important business metrics.

## 🔢 KPI Cards

The dashboard includes KPI cards for metrics such as:

* Total Sales
* Total Profit
* Total Orders
* Total Quantity
* Average Order Value
* Profit Margin %

## 📈 Pivot Charts

Pivot Charts were used to visualize:

* Sales trends
* Profit trends
* Category performance
* Regional performance
* Product performance
* Monthly/yearly performance
* Top-performing products
* Customer/segment performance

## 🎛️ Slicers

Interactive slicers allow users to dynamically analyze the data by dimensions such as:

* Year
* Month
* Region
* Category
* Product
* Customer
* Segment

## 🔍 Filters

Filters provide additional control over the dashboard and allow users to focus on specific:

* Time periods
* Categories
* Regions
* Products
* Customers
* Business segments

## 🎨 Dashboard Design

The dashboard was designed with:

* Clear KPI cards
* Interactive visualizations
* Consistent formatting
* User-friendly navigation
* Dynamic filtering
* Business-focused charts
* Easy-to-understand layouts

---

# 📸 Screenshots

## Dashboard

![Excel Dashboard](Screenshots/dashboard.png)

## Power Query

![Power Query](Screenshots/power-query.png)

## Power Pivot Data Model

![Power Pivot Data Model](Screenshots/data-model.png)

## DAX Measures

![DAX Measures](Screenshots/dax-measures.png)

> Add your actual screenshots to the `Screenshots` folder using the filenames shown above.

---

# 🔍 Key Findings

The dashboard was used to identify several business patterns and trends.

### 📈 Performance Trends

* Overall performance can be monitored across different time periods.
* Monthly and yearly trends help identify periods of growth or decline.
* KPI changes can be analyzed using interactive filters.

### 🏆 Product/Category Performance

* Top-performing products or categories can be identified.
* Low-performing products/categories can be investigated.
* Contribution to total sales and profit can be compared.

### 🌎 Regional Performance

* Performance can be compared across different regions.
* High- and low-performing regions can be identified.
* Regional trends can be analyzed using slicers.

### 💰 Profitability

* Sales and profit can be analyzed together.
* Profit margins can highlight differences in profitability.
* Areas with strong sales but comparatively lower profitability can be investigated.

### 👥 Customer/Segment Analysis

* Customer or segment performance can be compared.
* High-value segments can be identified.
* Performance can be analyzed dynamically using filters.

> **Important:** Replace these general findings with the specific numerical insights discovered in your dashboard.

---

# 🛠️ Tools & Technologies

| Tool / Feature      | Purpose                          |
| ------------------- | -------------------------------- |
| **Microsoft Excel** | Dashboard development            |
| **Power Query**     | Data cleaning and transformation |
| **Power Pivot**     | Data modeling                    |
| **DAX**             | KPI and analytical calculations  |
| **Pivot Tables**    | Data aggregation                 |
| **Pivot Charts**    | Data visualization               |
| **Slicers**         | Interactive filtering            |
| **Filters**         | Data exploration                 |

---

# 📁 Repository Structure

```text
Excel-Dashboard/
│
├── README.md
│
├── Dashboard/
│   └── Excel_Dashboard.xlsx
│
├── Data/
│   └── dataset.xlsx
│
├── Screenshots/
│   ├── dashboard.png
│   ├── power-query.png
│   ├── data-model.png
│   └── dax-measures.png
│
└── Documentation/
    └── DAX_Measures.txt
```

---

# 🚀 How to Use the Dashboard

1. Download or clone this repository.
2. Open `Excel_Dashboard.xlsx`.
3. Enable content/connections if Excel displays a security prompt.
4. Go to the **Dashboard** worksheet.
5. Use the available **Slicers and Filters**.
6. Select the required year, region, category, product, or other dimensions.
7. Review the KPI cards and Pivot Charts.
8. Explore the data to identify trends and business insights.

---

# 📚 Key Learning Outcomes

Through this project, I developed practical experience in:

* Data cleaning with Power Query
* Data transformation and preparation
* Data modeling with Power Pivot
* Writing DAX measures
* Creating dynamic KPIs
* Building Pivot Tables and Pivot Charts
* Creating interactive dashboards
* Using Slicers and Filters
* Business-oriented data analysis
* Presenting insights through data visualization

---

# ⭐ Project Highlights

```text
Power Query
     ↓
Data Cleaning
     ↓
Power Pivot
     ↓
Data Model
     ↓
DAX Measures
     ↓
Pivot Charts
     ↓
Slicers & Filters
     ↓
Interactive Dashboard
     ↓
Business Insights
```

This project demonstrates how **Microsoft Excel can be used as a complete data analytics and business intelligence tool**, combining data preparation, modeling, calculation, visualization, and interactive reporting in a single solution.

---

# 👤 Author

**Your Name**

**Skills:** Excel | Power Query | Power Pivot | DAX | Data Analysis | Data Visualization

---

## ⭐ If you found this project useful

If you found this project interesting or useful, consider giving the repository a **⭐ Star**.
