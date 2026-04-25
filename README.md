# 📊 World Layoffs: Data Cleaning & Exploratory Data Analysis (SQL)

In this project, I performed a complete data professional's workflow: from cleaning messy raw data to extracting deep business insights. This project showcases my ability to handle complex SQL operations and translate data into meaningful conclusions.

---

## 🛠️ Phase 1: Data Cleaning
The primary goal was to transform a raw dataset into a structured and reliable source.

### 📸 Visual Transformation
I cleaned the data by removing duplicates, standardizing naming conventions, and handling null values.

| Before Cleaning 

<img width="1064" height="350" alt="oncesi" src="https://github.com/user-attachments/assets/cca9ec89-2ae6-49cc-81e2-36389fe7c105" />
| After Cleaning |
<img width="1253" height="362" alt="sonrası" src="https://github.com/user-attachments/assets/52e792a2-92b4-4c3c-9427-742ebc2094ae" />

**Key Operations:**
* **De-duplication:** Used `ROW_NUMBER()` and CTEs to identify and remove redundant records.
* **Standardization:** Fixed industry names (e.g., 'Crypto') and removed trailing spaces.
* **Date Conversion:** Converted text-based dates into standard SQL `DATE` format.
* **Schema Optimization:** Dropped unnecessary columns like `row_num` after processing.

🔗 **[View Cleaning Script](./Data%20Cleaning%20Project.sql)**

---

## 🔍 Phase 2: Exploratory Data Analysis (EDA)
With a clean dataset, I explored the numbers to find the "story" behind the layoffs.

**Advanced Techniques Used:**
* **CTE & Window Functions:** To rank the top 5 companies with the most layoffs for each year.
* **Rolling Totals:** Calculated the cumulative layoff count month-by-month to see the progression of the "Tech Winter."
* **Aggregations:** Grouped data by industry, country, and funding stage to find the biggest losers.

🔗 **[View EDA Script](./Exploratory_Data_Analysis.sql)**

---

## 📈 Key Insights & Findings
* **The 2023 Peak:** My analysis confirmed that 2023 was far more devastating for tech employees than 2022.
* **Tech Giants:** Amazon, Google, and Meta recorded the largest individual layoff events.
* **Sector Volatility:** The Consumer and Retail sectors faced the most significant workforce reductions globally.
* **Funding Impact:** Companies in the "Post-IPO" stage accounted for the majority of the total layoffs.

---

## 💻 Tech Stack
* **Database:** MySQL / SQL Server
* **Core Skills:** CTEs, Window Functions (`DENSE_RANK`), Joins, Data Cleaning, Time-Series Analysis.

---

## 👨‍💻 Author
**Tunahan Oral**
*Management Information Systems Student at Alparslan Türkeş Science and Technology University*

[LinkedIn Profile](https://www.linkedin.com/in/tunahan-oral/) | [GitHub Portfolio](https://github.com/TunahanOral)
