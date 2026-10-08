![Power BI](https://img.shields.io/badge/Power%20BI-Data%20Analytics-yellow)
![Power Query](https://img.shields.io/badge/Power%20Query-Data%20Cleaning-blue)
![DAX](https://img.shields.io/badge/DAX-Measures-orange)
![Data Modeling](https://img.shields.io/badge/Data%20Modeling-Relationships-green)
![Status](https://img.shields.io/badge/Status-Completed-brightgreen)

# POWER BI SALES ANALYSIS DASHBOARD

A Power BI-based Sales Analysis project created using **Power BI Desktop**. The project focuses on cleaning and transforming raw data using **Power Query**, creating a structured data model, and developing **DAX measures** to analyze sales, customers, products, orders, and quantities.

---

## 📊 Project Overview

This project uses multiple datasets to build a structured sales analysis model and an interactive Power BI report.

The data was cleaned and transformed using **Power Query**, connected through relationships in the Power BI data model, and analyzed using custom **DAX measures**.

The final report provides insights into:

- Total Sales
- Total Orders
- Total Quantity
- Total Customers
- Average Order Value
- Sales Per Customer
- Electronics Sales
- Product Performance
- Customer Analysis
- Regional Analysis

---

## 🛠️ Tools & Technologies

- Microsoft Power BI Desktop
- Power Query
- DAX (Data Analysis Expressions)
- Data Modeling
- Data Visualization
- CSV Data Sources

---

## 📁 Dataset

The project uses four main datasets:

| Dataset | Records | Purpose |
|---|---:|---|
| Sales | 426 | Transaction and sales information |
| Customers | 20 | Customer details and regions |
| Products | 15 | Product information and categories |
| Dates | 365 | Date dimension for time-based analysis |

---

## 🗂️ Data Model

The project uses a relational data model consisting of:

```text
              ┌────────────┐
              │   Customers  │
              └─────┬──────┘
                     │
                     │ CustomerID
                     ▼
┌───────────┐  ┌───────────┐  ┌───────────┐
│    Dates    │  │    Sales    │  │   Products  │
└─────┬─────┘  └───────────┘  └─────┬─────┘
       │                                 │                 
       │ OrderDate                       │ ProductID       
       └────────────────────────────┘
```

The model allows sales transactions to be analyzed by:

- Date
- Customer
- Region
- Product
- Category

---

## 🧹 Data Cleaning with Power Query

Power Query was used to prepare the raw datasets before analysis.

The data preparation process included:

- Loading CSV datasets
- Reviewing data types
- Cleaning and transforming data
- Preparing tables for analysis
- Structuring the datasets for Power BI
- Creating a clean data model

---

## 🧮 DAX Measures

A dedicated `_Measures` table was created to organize the DAX measures used throughout the report.

### Measures Created

- **Total Sales**
- **Total Quantity**
- **Total Orders**
- **Total Customers**
- **Sales Per Customer**
- **Average Order Value**
- **Electronics Sales**

Example DAX measures include:

```DAX
Total Sales = SUM(Sales[Amount])
```

```DAX
Total Quantity = SUM(Sales[Quantity])
```

```DAX
Total Orders = DISTINCTCOUNT(Sales[OrderID])
```

```DAX
Total Customers = DISTINCTCOUNT(Sales[CustomerID])
```

The measures were created to make the report dynamic and allow calculations to respond to filters and visual interactions.

---

## 📈 Key Analysis Areas

### Sales Analysis

Analyze overall sales performance using:

- Total Sales
- Average Order Value
- Sales Per Customer

### Customer Analysis

Analyze:

- Total Customers
- Sales by Customer
- Customer contribution to sales

### Product Analysis

Analyze:

- Product performance
- Product categories
- Electronics sales
- Quantity sold

### Time Analysis

The dedicated Date table allows analysis by:

- Year
- Quarter
- Month
- Month Name
- Day
- Weekday

### Regional Analysis

Customer region information can be used to compare sales performance across different regions.

---

## 📊 Power BI Report

The final Power BI report provides an interactive environment where users can explore the data using filters, visualizations, and DAX-driven calculations.

### Key Dashboard Metrics

The report includes measures such as:

```text
Total Sales
Total Orders
Total Quantity
Total Customers
Average Order Value
Sales Per Customer
Electronics Sales
```

---

## 📸 Dashboard Preview

Add your Power BI dashboard screenshot here:

<img width="864" height="468" alt="image" src="https://github.com/user-attachments/assets/f2bb775a-c98b-4335-9dbf-ae6b4c96619a" />

---

## 📂 Project Structure

```text
power-bi-sales-analysis-dashboard/
│
├── Sales.csv
├── Customers.csv
├── Products.csv
├── Dates.csv
├── Power BI Sales Analysis.pbix
├── images/
│   └── power-bi-dashboard.png
└── README.md
```

---

## 📚 Skills Demonstrated

Through this project, I practiced and applied:

- Power BI Desktop
- Power Query
- Data Cleaning
- Data Transformation
- Data Modeling
- Table Relationships
- DAX
- DAX Measures
- KPI Development
- Data Visualization
- Interactive Reporting
- Business Data Analysis

---

## 🎯 Project Learning Outcomes

This project helped me understand how to take multiple raw datasets and transform them into a structured analytical model.

I gained practical experience in:

- Cleaning data using Power Query
- Building relationships between tables
- Creating a dedicated measures table
- Writing DAX measures
- Creating reusable calculations
- Analyzing sales and customer data
- Building interactive Power BI reports

---

## 🚀 Future Improvements

- Add year-over-year sales analysis
- Add month-over-month growth
- Add profit and profit margin analysis
- Add sales forecasting
- Add customer segmentation
- Add top/bottom product analysis
- Add advanced time-intelligence DAX measures
- Improve dashboard design and storytelling

---

## 👨‍💻 Author

**Navin Verma**

GitHub: https://github.com/Navin-Verma

---

⭐ If you found this project useful, consider giving it a star on GitHub!
