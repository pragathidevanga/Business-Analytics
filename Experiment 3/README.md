# 🛍️ Retail Sales & Performance Dashboard 📊

![Power BI](https://img.shields.io/badge/Power%20BI-Dashboard-yellow?style=for-the-badge&logo=powerbi)
![MySQL](https://img.shields.io/badge/MySQL-Database-blue?style=for-the-badge&logo=mysql)
![DAX](https://img.shields.io/badge/DAX-Data%20Analysis-orange?style=for-the-badge)
![Status](https://img.shields.io/badge/Project-Completed-success?style=for-the-badge)

## 📌 Project Overview

A retail company relies on manually prepared reports to monitor business performance. This project focuses on developing an interactive **Power BI dashboard** that provides a centralized view of retail sales and customer information.

The dashboard transforms raw business data into meaningful visual insights, helping users understand **sales performance, revenue, product performance, customer information, regional performance, and monthly trends**.

Instead of depending on manually prepared reports, the Power BI dashboard provides an interactive and user-friendly way to explore business performance.

---

## 🎯 Project Objective

The main objective of this project is to build a **Power BI Retail Sales & Performance Dashboard** that allows business users to:

- 📈 Monitor overall sales performance
- 💰 Analyze total revenue
- 🛒 Track total orders
- 👥 Understand customer information
- 🏷️ Analyze sales by product category
- 🌎 Compare sales across different regions
- 📅 Analyze monthly sales trends
- 🔎 Filter and explore data interactively
- 📊 Replace manual reporting with an interactive dashboard

---

## 🏢 Business Problem

The retail company currently depends on manually prepared reports to monitor its business performance.

Manual reporting can make it difficult to:

- ⏰ Access information quickly
- 📊 Identify sales trends
- 🔍 Analyze product performance
- 🌎 Compare regional performance
- 👥 Understand customer information
- 📈 Monitor changes in sales over time
- 🔄 Interactively filter and explore business data

To address these challenges, an interactive **Power BI dashboard** was developed.

---

# 🧩 Dataset & Data Sources

The project combines data from multiple sources to create a more complete business reporting solution.

### 🗄️ MySQL Database

The main retail transaction data is stored in a MySQL database.

The database contains tables such as:

### 🛒 Products Table

Contains information related to products:

- Product ID
- Product Name
- Category
- Price
- Supplier

### 💰 Sales Table

Contains retail sales transaction information:

- Sale ID
- Product ID
- Store ID
- Sale Date
- Quantity
- Total Amount

### 🏪 Stores Table

Contains information about retail stores:

- Store ID
- Store Name
- City
- State
- Store Type

### 👥 Customer Details

Additional customer information was incorporated into the Power BI model, including:

- Sale ID
- Customer ID
- Customer Name
- Gender
- Age
- Payment Method
- Customer Segment

---

# 🔗 Data Model

The Power BI data model connects sales transactions with customer information and other business dimensions.

The main relationship used for customer analysis is:

**Sales → Customer Details**

The relationship is based on:

retaildb sales[SaleID]
          ↕
Customer Details[SaleID]

This allows customer information to be analyzed together with sales transactions.

🛠️ Tools & Technologies

The following tools and technologies were used in this project:

📊 Power BI

Used to:

Import and transform data
Build the data model
Create DAX measures
Design interactive visualizations
Create the final dashboard
🗄️ MySQL

Used as the primary database for retail sales, product, and store information.

🧮 DAX

DAX (Data Analysis Expressions) was used to create analytical measures such as:

Total Sales =
SUM('retaildb sales'[TotalAmount])
Total Customers =
DISTINCTCOUNT('Customer Details'[CustomerID])
Customer Count =
COUNT('Customer Details'[CustomerID])
Average Customer Age =
AVERAGE('Customer Details'[Age])
📊 Dashboard Features

The dashboard provides several important business insights.

💰 1. Total Sales

The Total Sales KPI provides an overview of the total sales generated across the available retail transactions.

This helps management quickly understand the overall sales performance.

🛒 2. Total Orders

The Total Orders KPI shows the number of sales transactions.

This provides a quick understanding of the volume of business transactions.

👥 3. Total Customers

The Total Customers KPI provides the number of unique customers available in the customer dataset.

This helps provide insight into the customer base.

🏷️ 4. Sales by Category

The Sales by Category visualization compares sales performance across different product categories.

This can help identify:

⭐ High-performing categories
📉 Lower-performing categories
📊 Differences in category performance
🌎 5. Sales by Region

The dashboard includes regional sales analysis using store location information.

The store's State is used as the regional dimension.

This visualization helps identify:

🏆 Strong-performing regions
📉 Lower-performing regions
🌎 Geographic differences in sales performance
📅 6. Monthly Sales Trend

A monthly sales trend visualization is included to analyze how sales change over time.

This helps users identify:

📈 Increasing sales
📉 Decreasing sales
🔄 Seasonal patterns
📊 Changes in monthly performance
🎛️ Interactive Filters

The dashboard includes slicers that allow users to interactively filter the report.

📅 Month

Users can select a particular month or period.

🏷️ Category

Users can filter the dashboard based on product category.

🌎 Region

Users can filter the dashboard based on region/state.

When a filter is selected, the dashboard visuals update automatically.

🎨 Dashboard Design

The dashboard was designed with a clean and professional layout.

🎨 Background

A light grey background is used to provide a clean reporting environment.

⬜ Cards

White cards are used for important KPI values such as:

Total Sales
Total Orders
Total Customers
🖥️ Visual Layout

The dashboard follows a simple structure:

┌─────────────────────────────────────────────┐
│       🛍️ RETAIL SALES & PERFORMANCE        │
├────────────┬────────────┬───────────────────┤
│ 💰 Sales   │ 🛒 Orders  │ 👥 Customers      │
├────────────┴────────────┴───────────────────┤
│                                             │
│       📊 Sales by Category                  │
│                                             │
├──────────────────────┬──────────────────────┤
│ 🌎 Sales by Region   │ 📅 Monthly Trend     │
│                      │                      │
├──────────────────────┴──────────────────────┤
│ 🎛️ Month | Category | Region                │
└─────────────────────────────────────────────┘
📈 Key Business Insights

The dashboard enables business users to answer important questions such as:

💰 Sales Performance
What are the total sales?
How are sales changing over time?
Which periods generate higher sales?
🏷️ Product Performance
Which product categories generate the most sales?
Which categories require additional attention?
How does category performance compare?
🌎 Regional Performance
Which states/regions generate the highest sales?
Which regions have lower sales?
How does sales performance vary geographically?
👥 Customer Analysis
How many unique customers are there?
What is the average customer age?
What customer information is associated with transactions?
🧮 DAX Measures

Some of the key DAX measures used in the dashboard include:

💰 Total Sales
Total Sales =
SUM('retaildb sales'[TotalAmount])
👥 Total Customers
Total Customers =
DISTINCTCOUNT('Customer Details'[CustomerID])
👥 Customer Count
Customer Count =
COUNT('Customer Details'[CustomerID])
🎂 Average Customer Age
Average Customer Age =
AVERAGE('Customer Details'[Age])
🔄 Data Integration

One of the important aspects of this project is combining information from different data sources.

The project uses:

             🗄️ MySQL
                │
        ┌───────┼────────┐
        ↓       ↓        ↓
     Products  Sales   Stores
                │
                │
                ↕
        👥 Customer Details
                │
                ↓
          📊 Power BI
                │
                ↓
      🖥️ Interactive Dashboard

This approach allows multiple business dimensions to be analyzed within a single dashboard.

🚀 Project Workflow

The project was developed using the following workflow:

1️⃣ Data Collection

Retail sales, product, store, and customer data were collected.

2️⃣ Database Connection

The main retail data was connected from MySQL to Power BI.

3️⃣ Customer Data Integration

Customer details were incorporated into the Power BI model.

4️⃣ Data Modeling

Relationships between the relevant tables were created.

5️⃣ DAX Measures

Important business calculations were created using DAX.

6️⃣ Visualization

Charts, KPI cards, and slicers were added to the report.

7️⃣ Dashboard Design

The report was formatted with a clean and professional layout.

8️⃣ Final Dashboard

An interactive retail performance dashboard was created to replace manual reporting.

📁 Project Structure
📦 Retail-Sales-PowerBI
│
├── 📊 Retail_Sales_Dashboard.pbix
│
├── 📄 Retail_Customer_Details.csv
│
├── 🗄️ SQL/
│   ├── products.sql
│   ├── sales.sql
│   └── stores.sql
│
├── 📷 Dashboard/
│   └── dashboard_screenshot.png
│
└── 📖 README.md
💡 Benefits of the Dashboard

The Power BI dashboard provides several benefits to the retail business:

⚡ Faster Reporting

Reduces dependency on manually prepared reports.

📊 Better Visualization

Transforms raw data into easy-to-understand visual insights.

🔎 Interactive Analysis

Users can explore the data using filters and slicers.

📈 Trend Monitoring

Monthly trends can be monitored more easily.

🏷️ Product Analysis

Product categories can be compared to understand performance.

🌎 Regional Analysis

Sales performance can be analyzed by region.

👥 Customer Understanding

Customer information can be analyzed alongside sales data.

🎯 Better Decision Making

The dashboard provides a centralized view that can support business decision-making.

🎓 Project Outcome

The final result is an interactive Retail Sales & Performance Dashboard developed using Power BI.

The dashboard brings together sales, product, store, and customer information into one centralized reporting solution.

It provides business users with a simple way to monitor performance, identify trends, compare categories and regions, and explore customer information.

🏆 Conclusion

This project demonstrates how Power BI, MySQL, data modeling, and DAX can be used to transform manually prepared retail reports into an interactive business intelligence solution.

Instead of relying entirely on static reports, users can interact with the dashboard and quickly explore important business metrics.

The dashboard provides a foundation for:

📊 Data-driven decision making
📈 Sales performance monitoring
🏷️ Product category analysis
🌎 Regional performance analysis
👥 Customer analysis
📅 Trend analysis

🔮 Future Improvements

The dashboard can be further enhanced in the future with additional features such as:

💵 Profit and profit margin analysis
📦 Inventory analysis
🎯 Sales targets and achievement
📈 Year-over-Year (YoY) growth
📊 Customer segmentation analysis
🔄 Automated data refresh
📑 Drill-through reports
🚨 KPI alerts
☁️ Power BI Service deployment
👨‍💻 Skills Demonstrated

This project demonstrates practical experience in:

📊 Power BI
🗄️ MySQL
🧮 DAX
🔗 Data Modeling
📈 Data Visualization
🧹 Data Preparation
📊 Business Intelligence
📉 Sales Analysis
👥 Customer Analysis
🎨 Dashboard Design
⭐ Final Dashboard
🛍️ Retail Sales & Performance Dashboard

The completed dashboard provides a centralized and interactive view of retail business performance.

It replaces manually prepared reports with a visual, filterable, and easy-to-understand Power BI reporting solution.

🙌 Thank You

Thank you for visiting this project! 🚀

## 👨‍💻 Author

**Pragathi BR**

📊 Power BI Developer | Data Analyst  
🗄️ Power BI • MySQL • DAX • Data Visualization
