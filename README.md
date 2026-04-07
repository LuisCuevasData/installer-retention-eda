# Installer Retention EDA

**Capstone Project — IN498: Bachelor's Capstone in Analytics**
Purdue Global University | Luis Cuevas | April 2025

---

## Overview

This project was completed as part of my undergraduate analytics capstone at Purdue Global University. It focuses on data wrangling, exploratory data analysis (EDA), and data curation applied to mobile app installer retention data spanning nine months (April–December 2019).

The dataset tracks how many users who installed an app were still active at 1, 7, 15, 30, and 60 days post-install, broken down by country and month.

---

## Skills Demonstrated

- Parsing raw CSV files with inconsistent structure and mixed encodings (UTF-8 / UTF-16)
- Building reusable Python scripts for exploratory data analysis using pandas
- Merging multiple datasets into a single consolidated file
- Identifying and handling data quality issues (missing values, inconsistent date formats, empty strings)
- Documenting analytical decisions and methodology

---

## Project Structure

| File | Description |
|------|-------------|
| `IN498_LuisCuevas_Unit2.ipynb` | Main Jupyter notebook with all code, output, and written analysis |
| `IN498_Unit2_Student_Explorer.py` | Python script for individual file EDA |
| `IN498_Merge_and_Final_Explorer.py` | Python script for merging files and running final EDA |

---

## Key Findings

- All nine monthly files required parsing from a single-column raw format into properly structured 14-column DataFrames
- The mode for retained installers at every time interval (1, 7, 15, 30 days) was **0** across all files, consistent with typical mobile app churn patterns
- Mean retained installers declined progressively across retention windows, confirming a standard retention funnel
- October 2019 had the highest 1-day mean (3.08); September 2019 had the lowest (2.03) and fewest records (560)
- Data quality issues identified: one blank Country value in November 2019, inconsistent date formats (YYYY/MM/DD vs. YYYY-MM-DD) across files

---

## Tools & Libraries

- Python 3
- pandas
- Google Colab (Jupyter Notebook)
