# 🧹 Nashville Housing Data Cleaning in SQL

This project focuses on **cleaning and transforming raw housing data** in SQL Server using a variety of techniques. It’s part of my SQL portfolio, where I explore how to prepare real-world data for analysis and visualization.

---

## 📊 Project Overview

The dataset used contains information on property sales in Nashville. The main goal was to **clean and prepare the data for analysis** by performing operations like date formatting, address parsing, standardization, and removing duplicates.

---

## 🛠 Skills Used

- SQL Server  
- Data Cleaning & Preprocessing  
- Common Table Expressions (CTEs)  
- Window Functions  
- Data Type Conversion  
- CASE Statements  
- String Functions  
- Updating & Altering Tables  

---

## 🔧 Key Steps

### ✅ 1. Standardized Date Format  
Converted inconsistent date fields to proper `Date` format for easier filtering and timeline analysis.

### 🏠 2. Populated Missing Property Addresses  
Used self-joins to fill in missing `PropertyAddress` fields based on matching `ParcelID`.

### 🧱 3. Split Address Columns  
Used `SUBSTRING` and `CHARINDEX` to split `PropertyAddress` into:
- `PropertySplitAddress`  
- `PropertySplitCity`  

And used `PARSENAME` to split `OwnerAddress` into:
- `OwnerSplitAddress`  
- `OwnerSplitCity`  
- `OwnerSplitState`  

### ✔️ 4. Standardized Text Fields  
Transformed inconsistent "Y"/"N" values in the `SoldAsVacant` column into "Yes"/"No" for clarity using `CASE` statements.

### 🧹 5. Removed Duplicate Records  
Applied a `ROW_NUMBER()` window function within a CTE to identify and isolate duplicate entries based on multiple key fields.

### 🧼 6. Dropped Unused Columns  
Removed irrelevant or redundant columns (`OwnerAddress`, `TaxDistrict`, `PropertyAddress`, `SaleDate`) to streamline the dataset.

---

## 🗂 Data Source

The data was provided as part of a portfolio SQL project focused on housing sales in the Nashville area.

---

## ✅ How to Use

1. Clone this repository  
2. Load the SQL script into your SQL Server environment  
3. Execute each block step-by-step to clean the dataset  
4. Use the cleaned data for analysis or export to Power BI/Tableau  

---

## 👩‍💻 Author

**Immaculate Mary Nabuggwawo**  
_Data Analyst | Climate Tech Enthusiast_

🔗 [LinkedIn](https://www.linkedin.com/in/immaculate-nabuggwawo)  
📫 immaculate.nabuggwawo@gmail.com

---

