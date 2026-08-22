# 📊 README — Retail Business Intelligence Dashboard (MySQL → Power BI)

## 🏷️ Project Title
** Importing business datasets from flat files & MySQL and connecting with any other sources into Power BI**

## 📖 Project Overview
Retail businesses generate data across multiple disconnected systems — transactional sales records in a database, product catalogs, store location details, and customer information often stored separately in flat files. This project was built to solve exactly that problem: to design a centralized, reliable, and visually intuitive reporting system that brings all of this scattered data together into one place.

The project begins at the database layer, where a relational schema called **RetailDB** was designed and implemented in **MySQL Workbench**. This schema captures three core entities — Products, Stores, and Sales — each carefully structured with primary keys and appropriate data types to maintain integrity. On top of this, customer demographic data (gender, age, payment method, and customer segment) was sourced separately as a flat file, simulating a real-world scenario where not all business data lives in one system.

Once the database was populated and verified, the data was imported into **Power BI Desktop**, where it went through a full BI pipeline: cleaning and transformation via Power Query, relationship modeling via the Model view, DAX-based measure creation, and finally, visualization through an interactive, multi-page dashboard. The result is a working business intelligence tool that lets a retail manager instantly see total sales, orders, quantity sold, and customer counts, drill down by product category, city, store, or time period, and explore sales geographically through an interactive map. 🚀

## 🎯 Objectives
- 🗄️ Design a normalized relational database for retail operations in MySQL.
- 🔄 Import and integrate data from multiple heterogeneous sources (MySQL + flat file) into Power BI.
- 🧹 Clean, validate, and transform raw data to ensure reporting accuracy.
- 🔗 Build a proper data model with correct relationships between fact and dimension tables.
- ➗ Create meaningful DAX measures to power KPIs and visuals.
- 📊 Design an interactive, decision-ready dashboard for business stakeholders.

## 🗂️ Files Included
| 📄 File | 📝 Description |
|---|---|
| `RetailDB.sql` | 🛠️ SQL script that creates the RetailDB database and the Products, Stores, and Sales tables, along with sample INSERT statements |
| `Retail_Database_Assignment1.pbix` | 📈 Power BI Desktop file containing the imported tables, relationships, DAX measures, and the full 2-page dashboard |
| `Customer_Details.csv` | 👥 Flat file containing customer demographic data linked to sales via SaleID |
| 📃 Report (Word/PDF) | The full written report — problem statement, methodology (5 steps), screenshots, output, conclusion, and learning outcomes |

## 🧰 Tools & Technologies Used
- 🐬 **MySQL Workbench** — used for schema design, table creation, data insertion, and query execution
- 📊 **Power BI Desktop** — used for data import, modeling, DAX calculations, and dashboard/report building
- 🔧 **Power Query Editor** — used for data cleaning, type correction, duplicate removal, and column renaming
- ➗ **DAX (Data Analysis Expressions)** — used to define measures like Total Sales, Total Orders, Total Quantity, and Total Customers
- 🗺️ **Power BI Map Visual (Bing Maps integration)** — used to plot geographic sales data by city

## 🗃️ Database Schema
- 📦 **Products** → `ProductID` (PK), `Product Name`, `Category`, `Price`, `Supplier`
- 🏬 **Stores** → `StoreID` (PK), `Store Name`, `City`, `State`, `StoreType`
- 🧾 **Sales** → `SaleID` (PK), `ProductID` (FK), `StoreID` (FK), `SaleDate`, `Quantity`, `TotalAmount`
- 👤 **Customer Details** → `SaleID` (FK), `CustomerID`, `CustomerName`, `Gender`, `Age`, `PaymentMethod`, `CustomerSegment`

**Relationships:** Sales ↔ Products (via ProductID), Sales ↔ Stores (via StoreID), Sales ↔ Customer Details (via SaleID) — all one-to-many, with Sales as the central fact table. 🔗

## ▶️ How to Run This Project
1. 🐬 Open **MySQL Workbench** and run `RetailDB.sql` in a new query tab. This will drop any existing RetailDB, recreate it fresh, and populate all tables with sample data.
2. ✅ Verify the output log shows successful row insertions with 0 duplicates and 0 warnings.
3. 📂 Open **Power BI Desktop** and load `Retail_Database_Assignment1.pbix`.
4. 🔄 Go to **Home → Refresh** to make sure Power BI is pulling the latest data from your local MySQL instance.
5. 🖱️ Explore **Page 1** for the main dashboard (KPI cards, category chart, city chart, date trend) and **Page 2** for the interactive map view.
6. 🎚️ Use the **Month Year**, **Category**, and **City** slicers to filter and interact with the visuals in real time.

## ✨ Key Features
- 🔗 A centralized model combining structured (MySQL) and unstructured/flat-file (CSV) data sources.
- 🧩 Correctly modeled one-to-many relationships across four tables, avoiding ambiguous filter paths.
- 💳 KPI cards for **Total Sales (300.25K), Total Orders (18), Total Quantity (86), Total Customers (18)**.
- 🏆 Category-wise sales breakdown, showing Appliances as the top-performing category (168K).
- 🌆 City-wise sales comparison, with Mangalore leading at 84K in total sales.
- 📈 A date-based trend line tracking sales across September to November 2026.
- 🗺️ A fully interactive map visual plotting sales and orders across major Indian cities.
- 🎯 End-to-end interactivity — every visual responds to slicer selections, requiring zero technical knowledge from the end user.

## 🧪 Data Validation Checks Performed
- ✅ No duplicate records found across any of the four tables.
- ✅ No missing/null values in key fields (ProductID, StoreID, SaleID, CustomerID).
- ✅ Correct data types enforced (Date, Decimal, Whole Number) after import.
- ✅ Relationship cardinality verified as one-to-many in every case.

## 🎓 Learning Outcomes
- 🐬 Learned how to design and populate a relational database using MySQL from scratch.
- 🔌 Learned how to connect Power BI to both a live MySQL database and a flat-file source simultaneously.
- 🧹 Gained practical experience in data cleaning and transformation using Power Query.
- 🔗 Learned how to build and validate relationships across multiple tables, including a fact-to-fact style link.
- 🧮 Learned to write and apply DAX measures to power KPI cards and dynamic visuals.
- 📊 Learned how to design a clean, multi-page, interactive business dashboard suitable for real stakeholders.

## 🔮 Future Scope
- ➕ Add year-over-year and month-over-month growth measures using DAX time intelligence functions.
- 🤖 Integrate predictive analytics (e.g., sales forecasting) using Power BI's built-in forecasting feature.
- ☁️ Migrate the MySQL database to a cloud-hosted instance for real-time, always-available reporting.
- 📱 Optimize the report layout for mobile view using Power BI's mobile canvas designer.

## 👩‍💻 Author
**Pragathi BR**
🎓 Bachelor of Computer Applications (BCA), Semester V — Business Analytics
🏫 Department of Computer Application, Alliance University
📍 Chandapura–Anekal Main Road, Anekal, Bengaluru – 562106

---
