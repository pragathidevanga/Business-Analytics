# 📊 Superstore Sales Performance Analysis — Power BI Dashboard

## 🏷️ Project Title
**Sales Performance Analysis Across Products, Categories, and Regions using Power BI Visualizations**

## 📖 Overview
This project analyzes the **Sample Superstore dataset** to help retail management understand how sales and profit perform across different products, categories, and regions. Using **Power BI**, the raw transactional data (9,994 records) was imported, cleaned, modeled with a proper Date table, enriched with DAX measures, and transformed into a **3-page interactive dashboard** — giving stakeholders a clear, data-driven view of business performance from an overall, product-level, and regional perspective. 🚀

## 🎯 Objectives
- 📥 Import and prepare the Sample Superstore dataset for analysis in Power BI.
- 🧹 Clean and validate the data to ensure accuracy across all fields.
- 🔗 Build a robust data model with a dedicated Date table for time intelligence.
- ➗ Create reusable DAX measures to power every KPI and visual consistently.
- 📊 Design a multi-page, interactive dashboard highlighting sales, profit, and regional trends.

## 🗂️ Files Included
| 📄 File | 📝 Description |
|---|---|
| `Sample_Superstore.csv` | 📦 Raw dataset sourced from Kaggle (9,994 records, 13 fields) |
| `Superstore_Sales_Performance.pbix` | 📈 Power BI file with data model, DAX measures, and 3-page dashboard |
| 📃 Report (Word/PDF) | Full documented report — problem statement, methodology, screenshots, insights, and conclusion |

## 🧰 Tools & Technologies Used
- 📊 **Power BI Desktop** — data import, modeling, DAX, and dashboard design
- 🔧 **Power Query Editor** — data cleaning, type correction, and duplicate removal
- ➗ **DAX (Data Analysis Expressions)** — measure creation and time-intelligence calculations
- 🗺️ **Power BI Map Visual** — regional/state-level geographic analysis
- 📁 **Kaggle** — dataset source ([Sample Superstore](https://www.kaggle.com/))

## 🗃️ Dataset Details
- **Source:** Kaggle — Sample Superstore dataset
- **Records:** 9,994
- **Fields:** Ship Mode, Segment, Region, Category, Sub-Category, Sales, Quantity, Discount, Profit, and more

## 🔗 Data Modeling
- 📅 Built a dedicated **Date table** using `CALENDAR()` with Year, Month, Month Name, and Quarter columns.
- ✅ Marked it as an **official Date Table** in Power BI.
- 🔗 Created a **one-to-many relationship**: DateTable[Date] → Superstore[Order Date].
- 🧮 Verified correct cardinality in Model view.

## ➗ DAX Measures Created
```DAX
Total Sales = SUM(Superstore[Sales])
Total Profit = SUM(Superstore[Profit])
Profit Margin % = DIVIDE([Total Profit], [Total Sales], 0)
Total Orders = DISTINCTCOUNT(Superstore[Order ID])
Average Discount = AVERAGE(Superstore[Discount])
Total Quantity = SUM(Superstore[Quantity])
Sales Prior Year = CALCULATE([Total Sales], SAMEPERIODLASTYEAR(DateTable[Date]))
Sales YoY % = DIVIDE([Total Sales] - [Sales Prior Year], [Sales Prior Year], 0)
```

## 📑 Dashboard Pages

### 1️⃣ Executive Overview
- 💳 Four KPI cards: Total Sales (2.30M), Total Profit (286.41K), Profit Margin % (12.47%), Total Orders (5K).
- 📈 Line chart of Sales & Profit by Month.
- 🗺️ Map of Sales by State.
- 🎚️ Slicers for Year, Category, Region, Segment.

### 2️⃣ Category & Product Performance
- 📊 Bar chart: Sales by Sub-Category.
- ⚡ Scatter chart: Profit vs Discount by Sub-Category.
- 📋 Category-wise Sales, Profit & Margin table.
- 🏆 Top 10 Products by Sales table.

### 3️⃣ Regional Analysis
- 🗺️ Profit by State map (Red = Loss, Green = Profit).
- 📊 Column chart: Sales by Region and Segment.
- 📊 Bar chart: Sales by Ship Mode.
- 🍩 Donut chart: Sales by Segment.

## ✨ Key Insights & Findings
- 🎄 Sales spike sharply around November–December (holiday shopping).
- 📦 A small number of sub-categories drive most of the revenue.
- 🪑 Tables and Bookcases sell well but barely profit due to steep discounts.
- 📉 Higher discounts consistently correlate with lower profit.
- 🌎 West and East regions are the strongest performers; Central lags behind.
- 🏢 Corporate and Home Office segments are more profitable per sale than Consumer, despite lower volume.
- 🚚 Most orders ship via Standard Class, impacting delivery costs.
- 📆 Year-over-year comparison separates real growth from seasonal fluctuation.

## ▶️ How to Run
1. 📂 Download `Sample_Superstore.csv` and `Superstore_Sales_Performance.pbix`.
2. 📊 Open the `.pbix` file in **Power BI Desktop**.
3. 🔄 Click **Home → Refresh** if prompted, and update the data source path to your local CSV location if needed.
4. 🖱️ Navigate across the **Executive Overview**, **Category & Product Performance**, and **Regional Analysis** pages.
5. 🎚️ Use the slicers (Year, Category, Region, Segment) to explore the data interactively.

## 🎓 Learning Outcomes
- 📅 Learned to build a dedicated Date table and enable time intelligence in Power BI.
- 🧮 Gained hands-on experience with DAX functions: `SUM`, `DISTINCTCOUNT`, `DIVIDE`, `CALCULATE`, `SAMEPERIODLASTYEAR`.
- 🎨 Learned to design and format multiple visual types — KPI cards, line charts, bar charts, scatter charts, maps, and matrices.
- 🖌️ Practiced applying consistent themes and formatting for a professional, presentation-ready report.
- 💡 Learned to translate raw data patterns (like discount vs. profit) into actionable business insights.
- 📊 Improved end-to-end proficiency in Power BI — from data import to a finished, interactive dashboard.

## 👩‍💻 Author
**Prakruthi BR**
🎓 Bachelor of Computer Applications (BCA), Semester V — Business Analytics
🏫 Department of Computer Application, Alliance University
📍 Chandapura–Anekal Main Road, Anekal, Bengaluru – 562106
👨‍🏫 Faculty: Mr. Aman Kumar Sharma

---
