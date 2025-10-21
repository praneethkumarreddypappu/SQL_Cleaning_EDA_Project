# SQL Data Cleaning & Exploratory Data Analysis (EDA) – Layoffs Dataset

# Project Overview

This project demonstrates SQL techniques for **data cleaning and exploratory data analysis (EDA)** using a layoffs dataset. The goal is to transform messy, inconsistent raw data into a clean format and generate insights about industry trends, company layoffs, and regional impacts.

# Dataset

Source: Layoffs dataset (publicly available on Kaggle or similar open data repositories).
Files in this repo:

  * `data/raw/layoffs_sample.csv` → small sample of raw dataset (for reference).
  * `data/cleaned/layoffs_cleaned.csv` → cleaned version exported from SQL.

> ⚠️ Note: The full dataset is not included due to size limits. Only a sample is provided for reproducibility.

**Key columns:**
`company`, `location`, `industry`, `total_laid_off`, `percentage_laid_off`, `date`, `stage`, `country`, `funds_raised_millions`

---

## Project Structure

```
SQL-Layoffs-EDA/
│
├── data/
│   ├── raw/
│   │   └── layoffs_sample.csv
│   └── cleaned/
│       └── layoffs_cleaned.csv
│
├── sql/
│   ├── data_cleaning.sql       # Queries for cleaning
│   └── eda_queries.sql         # Queries for exploration
│
└── README.md
```

---

##  Data Cleaning Steps

* Removed duplicates and null values
* Standardized company and industry names
* Fixed inconsistent date formats
* Converted numerical columns to correct data types
* Filtered out invalid records (e.g., negative layoffs)

---

##  Exploratory Data Analysis (EDA)

* Layoffs by industry and company size
* Trends over time (monthly/yearly analysis)
* Layoffs by country and location
* Percentage of workforce laid off across industries
* Relationship between funding and layoffs

---

## Key Insights

* **Technology and Retail** sectors experienced the highest layoffs.
* **2022–2023** saw a significant spike in layoffs globally.
* Startups in **late funding stages** faced higher layoff percentages compared to early-stage companies.

---

## How to Use

1. Import the raw dataset into your SQL database.
2. Run the scripts in `sql/data_cleaning.sql` to prepare the dataset.
3. Use `sql/eda_queries.sql` to reproduce the exploratory analysis.
4. Compare results with the cleaned dataset provided.


