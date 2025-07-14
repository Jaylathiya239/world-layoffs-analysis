# world-layoffs-analysis

# 📉 Global Layoffs Data Analysis in MySQL

This project analyzes global layoffs data using MySQL, focusing on cleaning raw datasets and uncovering insights across companies, countries, and industries.

---

## 🧰 Skills & Tools Used

- MySQL
- Data Cleaning (TRIM, STR_TO_DATE, ISNULL)
- Window Functions (`ROW_NUMBER`, `DENSE_RANK`)
- Aggregations & Grouping
- CTEs, Subqueries

---

## 🧹 Phase 1: Data Cleaning

- **Removed Duplicate Records**  
  → Used `ROW_NUMBER()` to identify and delete duplicate entries.

- **Standardized Company Names**  
  → Applied `TRIM()` to remove leading/trailing whitespace.

- **Formatted Date Column**  
  → Converted text to `DATE` format using `STR_TO_DATE()` for consistency.

- **Handled Null Values**  
  → Removed rows with critical NULLs using `ISNULL()`.

- **Dropped Irrelevant Columns**  
  → Removed unneeded columns to improve clarity and query performance.

---

## 📊 Phase 2: Exploratory Data Analysis (EDA)

- **Max Layoffs & Max Percentage Laid Off**  
  → Found companies with highest layoff counts and layoff ratios.

- **Top Companies by Total Layoffs**  
  → Aggregated layoffs by company and ranked by total impact.

- **Layoff Time Span**  
  → Identified the earliest and latest layoff dates.

- **Layoffs by Industry**  
  → Highlighted industries most affected by job cuts.

- **Layoffs by Country**  
  → Ranked countries by total number of layoffs.

- **Top 5 Companies per Year**  
  → Used `DENSE_RANK()` to find the most affected companies annually.

---

## 🗃️ Data Source

- [Kaggle – Layoffs Dataset](https://www.kaggle.com/)  

---

## 📎 Notes

This project demonstrates how much business insight can be derived from structured SQL queries alone, with no external BI tools required. It’s designed as a backend-focused analysis showing practical SQL in action.
