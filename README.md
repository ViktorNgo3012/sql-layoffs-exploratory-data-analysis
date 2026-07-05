# SQL Exploratory Data Analysis Project – Layoffs Dataset

## Project Overview

This project demonstrates exploratory data analysis (EDA) using MySQL on a cleaned layoffs dataset. The analysis explores layoff trends across companies, industries, countries, funding stages, and time to better understand patterns in global workforce reductions.

Using SQL, the project summarises key metrics, compares business dimensions, analyses time-based trends, and ranks companies based on layoff activity. The analysis is performed on the cleaned dataset produced in the accompanying SQL Data Cleaning project.

---

## Dataset

The dataset contains information about company layoffs, including:

- Company
- Location
- Industry
- Total employees laid off
- Percentage of workforce laid off
- Date
- Funding stage
- Country
- Funds raised (millions)

---

## Analysis Objectives

This project aims to answer the following questions:

- Which companies experienced the largest layoffs?
- Which companies laid off 100% of their workforce?
- Which industries recorded the highest number of layoffs?
- Which countries were most affected by layoffs?
- How did layoffs change over time?
- How did layoffs differ across funding stages?
- Which companies recorded the highest layoffs each year?

---

## Exploratory Data Analysis Workflow

The analysis was performed through the following stages:

### 1. Dataset Overview

- Review the cleaned dataset.
- Identify the maximum number of layoffs.
- Identify the maximum layoff percentage.

### 2. Company Analysis

- Identify companies reporting complete workforce layoffs (100%).
- Calculate total layoffs by company.
- Calculate the average layoff percentage for each company.

### 3. Industry Analysis

- Analyse total layoffs across industries.

### 4. Country Analysis

- Analyse total layoffs by country.

### 5. Time Analysis

- Determine the overall date range.
- Analyse yearly layoffs.
- Analyse monthly layoffs.
- Calculate cumulative monthly layoffs using a rolling total.

### 6. Funding Stage Analysis

- Analyse layoffs across different funding stages.

### 7. Company Ranking

- Rank companies by yearly layoffs using the `DENSE_RANK()` window function.
- Identify the top five companies with the highest layoffs each year.

---

## SQL Skills Demonstrated

### SQL Querying

- `SELECT`
- `WHERE`
- `GROUP BY`
- `ORDER BY`

### Aggregate Functions

- `SUM()`
- `AVG()`
- `MAX()`
- `MIN()`

### Date Functions

- `YEAR()`
- `SUBSTRING()`

### SQL Techniques

- Common Table Expressions (CTEs)
- Window Functions (`SUM() OVER`)
- Ranking Functions (`DENSE_RANK()`)

### Data Analysis Techniques

- Aggregate analysis
- Trend analysis
- Time-series analysis
- Company ranking
- Business summarisation

---

## Key Insights Generated

The SQL analysis produces insights including:

- Companies with the largest workforce reductions.
- Companies reporting complete workforce layoffs.
- Industries with the highest total layoffs.
- Countries most affected by layoffs.
- Yearly layoff trends.
- Monthly layoff trends.
- Rolling cumulative layoffs over time.
- Layoff distribution across funding stages.
- Top five companies with the highest layoffs in each year.

---

## Project Structure

```text
sql-layoffs-exploratory-data-analysis/
│
├── layoffs_exploratory_data_analysis.sql
├── layoffs.csv
├── README.md
└── LICENSE
```

---

## Technologies Used

- MySQL
- SQL

---

## Future Improvements

- Extend the analysis with additional business metrics and comparative trends.
- Develop interactive dashboards in Power BI or Tableau based on the analysis.
- Expand the project with statistical and predictive analysis to further explore layoff patterns.
