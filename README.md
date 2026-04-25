# 📊 World Layoffs: Data Cleaning & Exploratory Data Analysis (SQL)

In this project, I performed a complete data professional's workflow: from cleaning messy raw data to extracting deep business insights using SQL. This project showcases my ability to handle complex database operations and translate raw numbers into meaningful conclusions.

---

## 🛠️ Phase 1: Data Cleaning
The primary goal was to transform a messy raw dataset into a structured, reliable, and analysis-ready source.

### 📸 Visual Transformation
I performed extensive cleaning, including removing duplicates, standardizing naming conventions, and fixing formatting issues.

| Raw Data (Before) 
<img width="1064" height="350" alt="oncesi" src="https://github.com/user-attachments/assets/6a63211d-2009-4fe2-8337-889a4399fb35" />
| Cleaned Data (After) |
<img width="1253" height="362" alt="sonrası" src="https://github.com/user-attachments/assets/ef9835ef-d229-4835-9771-0f75f44729b5" />


**Key Operations:**
* **De-duplication:** Identified and removed redundant records using `ROW_NUMBER()` and CTEs.
* **Standardization:** Fixed naming inconsistencies (e.g., 'Crypto' variants) and removed unnecessary white spaces.
* **Date Conversion:** Transformed text-based dates into standard SQL `DATE` format for time-series analysis.
* **Null Value Handling:** Populated missing industry data based on existing company records.

🔗 **[View Data Cleaning Script](./Data%20Cleaning%20Project.sql)**

---

## 🔍 Phase 2: Exploratory Data Analysis (EDA)
With a clean dataset, I explored the numbers to find the "story" behind the global layoffs.

**Advanced Techniques Used:**
* **Time-Series Analysis:** Calculated rolling totals of layoffs to visualize the cumulative impact month-by-month.
* **Advanced Ranking:** Used `DENSE_RANK()` and Window Functions to find the top 5 companies with the most layoffs for each specific year.
* **Aggregations:** Analyzed data by industry, country, and funding stage to identify the most affected sectors.

🔗 **[View EDA Script](./Exploratory_Data_Analysis.sql)**

---

## 📈 Key Insights & Findings
* **The 2023 Peak:** Analysis shows that 2023 was the most volatile year, significantly surpassing the total layoffs recorded in 2022.
* **Tech Giants Impact:** Major companies like Amazon, Google, and Meta led the charts in total layoffs during the post-pandemic adjustment.
* **Sector Analysis:** The Consumer and Retail industries faced the most significant workforce reductions globally.
* **Funding Stages:** Companies in the "Post-IPO" stage accounted for the vast majority of total layoffs compared to early-stage startups.

---

## 💻 Tech Stack
* **Database:** MySQL / SQL Server
* **Core Skills:** CTEs, Window Functions, Joins, Data Cleaning, Aggregate Functions.

---

## 👨‍💻 Author
**Tunahan Oral**
*Management Information Systems Student at Alparslan Türkeş Science and Technology University*

[LinkedIn Profile](https://www.linkedin.com/in/tunahan-oral/) | [GitHub Portfolio](https://github.com/TunahanOral)
