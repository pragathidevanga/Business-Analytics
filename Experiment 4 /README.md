# ☕ Dirty Cafe Sales Data Cleaning and Preparation Using Power Query

![Power BI](https://img.shields.io/badge/Power%20BI-Data%20Cleaning-yellow?style=for-the-badge\&logo=powerbi)
![Power Query](https://img.shields.io/badge/Power%20Query-ETL-blue?style=for-the-badge)
![Kaggle](https://img.shields.io/badge/Dataset-Kaggle-20BEFF?style=for-the-badge\&logo=kaggle)
![CSV](https://img.shields.io/badge/Data-CSV-orange?style=for-the-badge)
![Business Analytics](https://img.shields.io/badge/Domain-Business%20Analytics-green?style=for-the-badge)

## 📌 Project Overview

This project focuses on **cleaning and preparing a dirty cafe sales dataset using Power Query in Microsoft Power BI**.

Real-world business datasets often contain problems such as **missing values, errors, inconsistent text, incorrect data types, duplicate records, invalid numerical values, and unstructured entries**. Before performing any business analysis or visualization, these issues need to be identified and corrected.

In this project, the **Dirty Cafe Sales Dataset** was imported into Power BI and processed using **Power Query Editor**. A series of data-cleaning and transformation operations were performed to improve the quality, consistency, and usability of the dataset.

The main objective of the project is to demonstrate how **Power Query can be used as an ETL (Extract, Transform, Load) tool** for preparing raw business data for analysis.

---

## 🎯 Project Objectives

The major objectives of this project are:

* 🧹 Clean a raw and inconsistent cafe sales dataset.
* 🔍 Identify errors, missing values, duplicate records, and inconsistent entries.
* 🔄 Transform columns into appropriate formats.
* ✏️ Standardize inconsistent text values.
* 💰 Correct and prepare numerical sales-related fields.
* 📅 Filter and prepare transaction date information.
* 🧮 Create calculated values where required.
* 🗑️ Remove unnecessary or old columns.
* 📑 Reorder and rename columns for better readability.
* 🔢 Validate numerical values such as Quantity and Price Per Unit.
* ✨ Trim and clean unwanted spaces from text fields.
* 📊 Prepare the final dataset for future business analysis.

---

## 📂 Dataset

The dataset used in this project is the **Dirty Cafe Sales Dataset**, obtained from Kaggle.

🔗 **Dataset Source:**
[Kaggle – Dirty Cafe Sales Dataset](https://www.kaggle.com/search?q=Dirty+Cafe+Sales+Dataset)

The dataset contains cafe transaction-level information such as items purchased, quantity, price, payment method, location, and transaction date.

---

## 📋 Dataset Description

The Dirty Cafe Sales Dataset represents sales transactions from a cafe environment.

Each row represents a **sales transaction**, while each column represents a particular attribute related to that transaction.

The raw dataset contains several data-quality problems intentionally included for cleaning practice. These problems make the dataset suitable for demonstrating practical **data preprocessing and transformation techniques**.

### 📊 Dataset Information

| Attribute          | Description                     |
| ------------------ | ------------------------------- |
| 📁 Dataset         | Dirty Cafe Sales Dataset        |
| 🏪 Domain          | Cafe Sales / Business Analytics |
| 📄 File Format     | CSV                             |
| 🔧 Processing Tool | Microsoft Power BI              |
| 🧹 Cleaning Tool   | Power Query Editor              |
| 📊 Data Type       | Transactional Sales Data        |
| 🎯 Main Purpose    | Data Cleaning and Preparation   |

---

## 🧾 Dataset Columns

The dataset contains the following major columns:

| Column Name         | Description                                             |
| ------------------- | ------------------------------------------------------- |
| 🆔 Transaction ID   | Unique identifier associated with each cafe transaction |
| ☕ Item              | Name of the product purchased                           |
| 🔢 Quantity         | Number of units purchased                               |
| 💵 Price Per Unit   | Price of one unit of the selected item                  |
| 💰 Total Spent      | Total amount spent in the transaction                   |
| 💳 Payment Method   | Method used by the customer for payment                 |
| 📍 Location         | Location associated with the transaction                |
| 📅 Transaction Date | Date on which the transaction occurred                  |

---

# ⚠️ Data Quality Issues

The raw dataset contained several issues that required preprocessing before analysis.

The cleaning process addressed issues such as:

* ❌ Errors in the **Total Spent** column.
* ❓ Unknown or inconsistent values in **Payment Method**.
* 🔢 Incorrect or inconsistent data types.
* 🔁 Duplicate **Transaction ID** records.
* 📝 Inconsistent item names.
* 📍 Inconsistent location values.
* 💳 Payment method inconsistencies.
* 📅 Transaction date filtering requirements.
* 🧮 Invalid or unsuitable Quantity values.
* 💵 Invalid Price Per Unit values.
* ✂️ Extra spaces in text fields.
* 🧹 Unclean text entries.
* 🗑️ Unnecessary old columns.
* 🔄 Columns requiring renaming and reordering.

These problems were handled using Power Query transformations.

---

# 🛠️ Tools and Technologies

### 💻 Microsoft Power BI

Microsoft Power BI was used as the primary platform for importing, transforming, and preparing the dataset.

### 🔧 Power Query

Power Query Editor was used to perform the complete data-cleaning process.

Operations included:

* Changing data types
* Replacing errors
* Replacing unknown values
* Adding columns
* Removing columns
* Renaming columns
* Replacing values
* Filtering records
* Removing duplicates
* Reordering columns
* Trimming text
* Cleaning text
* Validating numerical fields

### 📁 CSV

The original dataset was provided in CSV format and imported into Power BI for transformation.

### 🌐 Kaggle

Kaggle was used as the source of the Dirty Cafe Sales Dataset.

---

# 🔄 Methodology

The project follows a structured data-cleaning workflow:

```text
📥 Raw Dataset
      ↓
☕ Dirty Cafe Sales Dataset
      ↓
📊 Import into Power BI
      ↓
🔧 Power Query Editor
      ↓
🧹 Data Cleaning
      ↓
🔄 Data Transformation
      ↓
🔍 Data Validation
      ↓
✨ Cleaned Dataset
      ↓
📊 Ready for Analysis
```

---

# 📌 Step 1 – Data Collection

The Dirty Cafe Sales Dataset was collected from Kaggle.

The dataset was selected because it contains several common data-quality problems found in real-world business datasets.

The raw data was used as the starting point for the Power Query cleaning process.

The dataset contains transaction-level information related to:

* Customer purchases
* Items
* Quantity
* Unit price
* Total spending
* Payment methods
* Locations
* Transaction dates

The objective at this stage was to obtain the original raw dataset without manually modifying it before importing it into Power BI.

---

# 📥 Step 2 – Data Import

The dataset was imported into **Microsoft Power BI**.

After opening Power BI, the CSV dataset was loaded and opened in **Power Query Editor**.

Power Query provides a separate environment where the raw dataset can be inspected and transformed without directly modifying the original source file.

The imported columns were reviewed to understand:

* Column names
* Existing data types
* Missing or unknown values
* Error values
* Text inconsistencies
* Numerical inconsistencies
* Duplicate transactions

This inspection helped determine the cleaning operations required for the dataset.

---

# 🧹 Step 3 – Data Cleaning and Transformation

The main part of the project was completed in Power Query Editor.

A total of **23 applied transformation steps** were used to clean and prepare the dataset.

## 🔢 Applied Steps

### 1️⃣ Source

The original Dirty Cafe Sales Dataset was connected to Power Query.

This step represents the source connection from which the raw dataset was loaded.

---

### 2️⃣ Set Columns to Text – All Columns

All columns were initially converted to **Text** format.

This helped provide a consistent starting point before performing further transformations.

It also allowed errors and inconsistent entries to be handled during the cleaning process.

---

### 3️⃣ Promoted Headers – First Row

The first row of the dataset was promoted as the column headers.

This ensured that the actual field names were correctly recognized by Power Query.

The resulting columns included:

* Transaction ID
* Item
* Quantity
* Price Per Unit
* Total Spent
* Payment Method
* Location
* Transaction Date

---

### 4️⃣ Set Data to Text – All Columns

The dataset columns were again assigned the **Text** data type as part of the transformation process.

This provided a consistent format while handling errors and values before assigning the final appropriate data types.

---

### 5️⃣ Replaced Errors – Total Spent

Errors found in the **Total Spent** column were replaced.

This step was necessary because invalid values in a numerical sales field can affect calculations and analysis.

The Total Spent column was prepared for subsequent transformation.

---

### 6️⃣ Replaced Unknowns – Payment Method

Unknown or unsuitable values in the **Payment Method** column were handled.

This improved the consistency of payment-related information and reduced unwanted unknown entries.

---

### 7️⃣ Changed Data Types – Quantity

The **Quantity** column was converted to an appropriate numerical data type.

Since Quantity represents the number of products purchased, treating it as a numerical field is necessary for analysis and validation.

---

### 8️⃣ Added Total Spent

A new **Total Spent** calculated column was added during the transformation process.

This helped prepare a usable sales-value field from the available transaction information.

---

### 9️⃣ Added Quantity

A new **Quantity** column was added as part of the transformation process.

This ensured that the required quantity information was available in the prepared dataset.

---

### 🔟 Added Unit Price

A new **Unit Price** column was created.

This helped organize the price-related information in a clearer and more usable form.

---

### 1️⃣1️⃣ Removed Old Columns

The older or unnecessary versions of the columns were removed.

This prevented duplicate information from remaining in the final dataset and made the table easier to work with.

---

### 1️⃣2️⃣ Renamed Columns for New Calculated Columns

The newly created columns were renamed appropriately.

Clear column names make the final dataset easier to understand and use for future analysis.

---

### 1️⃣3️⃣ Replaced Item Values

Inconsistent values in the **Item** column were standardized.

This ensured that the same product was represented consistently throughout the dataset.

Standardized item names are important when calculating product-level sales or creating visualizations.

---

### 1️⃣4️⃣ Renamed Payment Method

The payment-related column was renamed to provide a clear and standardized field name.

This improved readability and consistency in the final dataset.

---

### 1️⃣5️⃣ Replaced Location

Inconsistent values in the **Location** column were replaced or standardized.

This helped ensure that location-based analysis could be performed more reliably.

---

### 1️⃣6️⃣ Filtered Dates – Transaction Date

The **Transaction Date** field was filtered to prepare valid transaction records.

Date filtering helps remove unsuitable date entries and ensures that the resulting dataset contains usable transaction-date information.

---

### 1️⃣7️⃣ Removed Duplicates – Transaction ID

Duplicate records based on **Transaction ID** were removed.

A Transaction ID is used to identify a transaction, so duplicate records can lead to incorrect calculations and misleading business insights.

Removing duplicate Transaction IDs helped improve data integrity.

---

### 1️⃣8️⃣ Reordered Columns

The columns were reordered into a more logical sequence.

This improved the readability and organization of the final dataset.

---

### 1️⃣9️⃣ Updated Data Types

The columns were assigned their appropriate final data types.

For example:

* Quantity → Numerical
* Price Per Unit → Numerical
* Total Spent → Numerical
* Transaction Date → Date
* Item → Text
* Payment Method → Text
* Location → Text

Correct data types are essential for accurate calculations and future analysis.

---

### 2️⃣0️⃣ Trimmed Text – Item, Payment Method and Location

The **Item, Payment Method, and Location** columns were trimmed.

The Trim operation removes unnecessary spaces before or after text values.

This helps avoid situations where visually identical values are treated as different values because of hidden spaces.

---

### 2️⃣1️⃣ Cleaned Text – Item, Payment Method and Location

The text fields were cleaned to remove unwanted or non-printable characters.

The cleaning operation was applied to:

* Item
* Payment Method
* Location

This improved the quality and consistency of textual data.

---

### 2️⃣2️⃣ Filtered Quantity

The **Quantity** field was filtered to remove unsuitable or invalid numerical entries.

This ensured that the Quantity column contained usable values for further analysis.

---

### 2️⃣3️⃣ Filtered Price Per Unit

The **Price Per Unit** field was filtered to remove unsuitable values.

This helped ensure that price information was appropriate for calculations and business analysis.

---

# 📋 Applied Steps Summary

| No. | Applied Step                       | Purpose                              |
| --: | ---------------------------------- | ------------------------------------ |
|   1 | Source                             | Connect raw dataset                  |
|   2 | Set Columns to Text                | Standardize initial data format      |
|   3 | Promoted Headers                   | Set first row as headers             |
|   4 | Set Data to Text                   | Maintain consistent text format      |
|   5 | Replaced Errors – Total Spent      | Handle sales-value errors            |
|   6 | Replaced Unknowns – Payment Method | Handle unknown payment entries       |
|   7 | Changed Data Types – Quantity      | Convert Quantity to numerical format |
|   8 | Added Total Spent                  | Create prepared sales-value field    |
|   9 | Added Quantity                     | Create prepared quantity field       |
|  10 | Added Unit Price                   | Create prepared price field          |
|  11 | Removed Old Columns                | Remove unnecessary columns           |
|  12 | Renamed Columns                    | Improve column naming                |
|  13 | Replaced Item Values               | Standardize item values              |
|  14 | Renamed Payment Method             | Improve field naming                 |
|  15 | Replaced Location                  | Standardize location values          |
|  16 | Filtered Dates                     | Prepare valid transaction dates      |
|  17 | Removed Duplicates                 | Remove duplicate transactions        |
|  18 | Reordered Columns                  | Improve table organization           |
|  19 | Updated Data Types                 | Apply final data types               |
|  20 | Trimmed Text                       | Remove unwanted spaces               |
|  21 | Cleaned Text                       | Remove unwanted characters           |
|  22 | Filtered Quantity                  | Remove unsuitable quantity values    |
|  23 | Filtered Price Per Unit            | Remove unsuitable price values       |

---

# 🔍 Step 4 – Final Data Validation and Preparation

After applying all cleaning and transformation operations, the final dataset was reviewed in Power Query.

The purpose of validation was to make sure that the cleaning operations had been successfully applied.

The following aspects were checked:

### ✅ Column Structure

The final dataset was checked to confirm that unnecessary columns had been removed and required columns were available.

### ✅ Data Types

The final data types were reviewed to ensure that numerical, text, and date fields were appropriately formatted.

### ✅ Duplicate Records

Transaction ID values were checked after applying the duplicate-removal operation.

### ✅ Text Consistency

Item, Payment Method, and Location fields were reviewed after trimming and cleaning.

### ✅ Numerical Values

Quantity, Price Per Unit, and Total Spent were reviewed after filtering and transformation.

### ✅ Date Values

Transaction Date was reviewed after applying the required date filtering.

---

# 📸 Screenshots / Figures

Screenshots can be added to document the Power Query process.

### Fig. 1 – Kaggle Dirty Cafe Sales Dataset

*Raw dataset used for the cleaning process.*

### Fig. 2 – Dataset Imported into Power Query

*Dataset loaded into Power Query Editor.*

### Fig. 3 – Data Cleaning and Transformation in Power Query

*Applied transformations used to clean the dataset.*

### Fig. 4 – Validation of Cleaned Dataset

*Final dataset checked after transformation.*

### Fig. 5 – Final Cleaned Dataset

*Prepared dataset ready for analysis.*

---

# 📊 Output

The final output of this project is a **cleaned and structured cafe sales dataset**.

The original raw dataset contained various data-quality issues, including errors, unknown values, duplicate records, inconsistent text, and unsuitable numerical entries.

After processing the dataset through Power Query, the data was transformed into a more consistent and analysis-ready format.

## 🔴 Before Cleaning

The original dataset contained:

* Data errors
* Unknown values
* Duplicate Transaction IDs
* Inconsistent item values
* Inconsistent location values
* Inconsistent payment method entries
* Incorrect data types
* Unwanted spaces
* Unclean text
* Unsuitable Quantity values
* Unsuitable Price Per Unit values

## 🟢 After Cleaning

The prepared dataset contains:

* Standardized column names
* Appropriate data types
* Cleaner text values
* Improved payment method consistency
* Standardized item values
* Standardized location values
* Valid transaction-date entries
* Duplicate Transaction IDs removed
* Prepared numerical fields
* Organized column structure
* Cleaner values suitable for analysis

---

# 📈 Data Cleaning Summary

| Data Quality Issue          | Power Query Operation | Result                  |
| --------------------------- | --------------------- | ----------------------- |
| ❌ Errors in Total Spent     | Replace Errors        | Errors handled          |
| ❓ Unknown Payment Method    | Replace Values        | Values standardized     |
| 🔢 Incorrect Quantity Type  | Change Data Type      | Numerical format        |
| 💰 Sales Field Preparation  | Add Total Spent       | Prepared sales field    |
| 🔢 Quantity Preparation     | Add Quantity          | Prepared quantity field |
| 💵 Price Preparation        | Add Unit Price        | Prepared price field    |
| 🗑️ Unnecessary Fields      | Remove Columns        | Cleaner dataset         |
| ✏️ Inconsistent Item Values | Replace Values        | Standardized items      |
| 📍 Location Issues          | Replace Values        | Standardized locations  |
| 📅 Date Issues              | Filter Dates          | Valid date records      |
| 🔁 Duplicate Transactions   | Remove Duplicates     | Improved uniqueness     |
| ↔️ Poor Column Order        | Reorder Columns       | Organized table         |
| 📝 Extra Spaces             | Trim                  | Cleaner text            |
| 🧹 Unwanted Characters      | Clean                 | Clean text              |
| 🔢 Invalid Quantity         | Filter Quantity       | Suitable values         |
| 💵 Invalid Unit Price       | Filter Price          | Suitable values         |

---

# 💡 Key Learning Outcomes

Through this project, I gained practical knowledge of **Power Query and data preprocessing**.

### 🧹 Data Cleaning

I learned how to identify and handle common data-quality issues such as errors, duplicate records, missing or unknown values, and inconsistent entries.

### 🔄 Data Transformation

I learned how Power Query can transform raw data into a structured format suitable for analysis.

### 🔢 Data Types

I understood the importance of assigning appropriate data types to numerical, text, and date columns.

### ✏️ Text Cleaning

I learned how to use **Trim** and **Clean** operations to improve text consistency.

### 🔁 Duplicate Removal

I learned how duplicate transaction records can affect data accuracy and how to remove duplicates using Power Query.

### 🔍 Data Validation

I learned how to review and validate transformed data before using it for business analysis.

### 📊 Business Analytics Preparation

The project helped me understand that accurate business analysis depends on the quality of the underlying data.

---

# 🎯 Conclusion

The **Dirty Cafe Sales Data Cleaning and Preparation Using Power Query** project demonstrates the importance of data preprocessing in Business Analytics.

The raw Dirty Cafe Sales Dataset contained several data-quality issues, including errors, unknown values, duplicate records, inconsistent text values, unsuitable numerical values, and data-type problems.

Using **Power Query in Microsoft Power BI**, these issues were addressed through a structured series of transformation operations. The process included replacing errors and unknown values, changing data types, creating required columns, standardizing text values, removing duplicates, filtering records, trimming and cleaning text, and organizing the final table.

The resulting dataset is cleaner, more consistent, and better prepared for future business analysis and visualization.

This project provided practical experience in using **Power Query as an ETL and data-preparation tool** and strengthened my understanding of how raw business data can be converted into reliable analytical data.

---

# 🗂️ Project Structure

```text
☕ DIRTY-CAFE-SALES-DATA-CLEANING-USING-POWER-QUERY
│
├── 📄 README.md
│
├── 📂 Dataset
│   └── Dirty_Cafe_Sales_Dataset.csv
│
├── 📂 PowerBI
│   └── Dirty_Cafe_Sales_Data_Cleaning.pbix
│
├── 📂 Report
│   └── Dirty_Cafe_Sales_Data_Cleaning_Report.pdf
│
└── 📂 Screenshots
    ├── 01_Dataset_Before_Cleaning.png
    ├── 02_Power_Query_Editor.png
    ├── 03_Applied_Steps.png
    ├── 04_Data_Validation.png
    └── 05_Final_Cleaned_Dataset.png
```

---

# 🧰 Technologies Used

| Technology            | Purpose                          |
| --------------------- | -------------------------------- |
| 📊 Microsoft Power BI | Data import and processing       |
| 🔧 Power Query        | Data cleaning and transformation |
| 📄 CSV                | Dataset format                   |
| 🌐 Kaggle             | Dataset source                   |
| 📈 Business Analytics | Project domain                   |

---

# 🔗 Project Links

### 🌐 Dataset Source

👉 [**Dirty Cafe Sales Dataset – Kaggle**](https://www.kaggle.com/search?q=Dirty+Cafe+Sales+Dataset)

---

# 👩‍💻 Author

### **Pragathi BR**

🎓 **Bachelor of Computer Applications (BCA)**
🤖 **Artificial Intelligence & Machine Learning**
🏫 **Alliance University, Bengaluru**
📊 **Area: Business Analytics / Data Analytics**

---

## ⭐ Project Highlights

✨ Practical Power Query data-cleaning project
✨ 23 documented transformation steps
✨ Error handling and data validation
✨ Duplicate removal
✨ Text standardization
✨ Numerical data filtering
✨ Data-type transformation
✨ Transaction date preparation
✨ Dataset preparation for business analysis
✨ Developed using Microsoft Power BI

---

## 🙌 Acknowledgement

I would like to acknowledge **Kaggle** for providing the dataset used for this project and **Alliance University** for providing the academic platform to develop practical knowledge in Business Analytics and Power BI.

---

## ⭐ If you found this project useful

If this project helped you understand **Power Query data cleaning and transformation**, feel free to ⭐ the repository and explore the project files.

---

### 📌 Final Project Title

> **Dirty Cafe Sales Data Cleaning and Preparation Using Power Query**

**Made with ☕ + 📊 + 🔧 Power Query**
**© 2026 Pragathi BR**
