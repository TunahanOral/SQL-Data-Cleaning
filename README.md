# 🧹 SQL Data Cleaning Project: Global Layoffs Dataset

## 🎯 Objective
In this project, I transformed a raw, messy dataset containing global tech and industry layoffs into a clean, standardized format ready for Exploratory Data Analysis (EDA) and Business Intelligence (BI) dashboards. As a data analyst, I know that visualizing dirty data leads to flawed business decisions, so ensuring data integrity was my top priority.

## 🛠️ Tools & SQL Techniques Used

**1. Data Staging (Security First)**
* Created a `layoffs_staging` table to act as a sandbox. I performed all cleaning operations on this backup table to preserve the integrity of the raw database.

**2. Removing Duplicates**
* Utilized **Window Functions** (`ROW_NUMBER() OVER(PARTITION BY ...)`) paired with **Common Table Expressions (CTEs)** to identify and delete completely identical rows without losing unique data.

**3. Data Standardization**
* **String Manipulation:** Applied `TRIM()` functions to remove trailing spaces and punctuation from company names and locations (e.g., changing 'United States.' to 'United States').
* **Category Grouping:** Used the `LIKE` operator to consolidate varying industry names (e.g., unifying different 'Crypto' tags).
* **Data Type Conversion:** Converted the date column from text/string format into a standard `DATE` format using `STR_TO_DATE()` for accurate time-series analysis.

**4. Handling NULL and Blank Values**
* **Data Recovery via Self Join:** Identified companies with missing `industry` values and populated them by performing a `JOIN` on the same table, extracting the missing data from other branches of the same company.
* **Dropping Unusable Data:** Deleted rows where both `total_laid_off` and `percentage_laid_off` were NULL, as these rows provided no mathematical value for future aggregations.

## 📸 Before & After

**🔴 Raw Data (Contains duplicates, unformatted dates, and blanks)**
<img width="1064" height="350" alt="oncesi" src="https://github.com/user-attachments/assets/6f8380b3-3eab-43b8-a0e5-d6b9c7a70f0b" />


**🟢 Cleaned & Ready for Analysis**
<img width="1253" height="362" alt="sonrası" src="https://github.com/user-attachments/assets/072e63fb-941e-4ba0-ac0a-c2c9e342bb03" />
