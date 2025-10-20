# Nigeria Inflation Data Analysis  

## Overview  
This project explores Nigeria’s inflation trends using publicly available data.  
The main goal was to **clean**, **verify**, and **analyze** the dataset to understand how inflation behaves over time and how it relates to key economic factors such as crude oil prices and exports.  

---

## Data Source  
- **Primary:** [Kaggle – Nigeria Inflation Dataset](https://www.kaggle.com/)  
- **Verification:** Central Bank of Nigeria (CBN) official statistics  

---

## Data Cleaning & Preparation  
The dataset was cleaned and prepared for analysis to ensure accuracy and consistency.  

**Key steps:**  
- Imported all necessary Python libraries (Pandas, NumPy, Matplotlib, Seaborn)  
- Loaded and inspected the dataset  
- Checked for missing values and handled them appropriately  
  - April 2023 had missing values for `Crude Oil Price`, `Production`, and `Crude Oil Export`  
  - Filled missing values using official CBN data  
- Checked for duplicates and corrected data types  
- Combined **Year** and **Month** columns into a single **Date** column  
- Added a `Day=1` column to form valid date objects  
- Filtered dataset to cover the **2015–2024** period for consistency  

---

## Feature Engineering  
New variables were created to enrich the analysis:  
- **Inflation_Change:** Month-to-month difference in inflation rate  
- **Trend:** Categorized as *Rising*, *Falling*, or *Stable*  
- **Date:** Combined year-month column for time-series visualization  
- Converted numeric months (1–12) to abbreviations *(Jan, Feb, Mar, …, Dec)*  

---

## Exploratory Data Analysis (EDA)  
Statistical and correlation analysis was conducted to understand inflation behavior.

**EDA Highlights:**  
- Identified **maximum and minimum** inflation values and their years  
- Computed **average**, **standard deviation**, and **summary statistics**  
- Calculated **average inflation rate** for each year and month  
- Measured **year-over-year (%) changes** in inflation  
- Analyzed **average monthly trends** across all years  
- Compared inflation with **Crude Oil Price**, **Production**, and **Exports**  
- Calculated **z-scores** to detect statistical outliers (|z| > 2)  
- Quantified the difference between % change in **inflation rate** and % change in **crude oil price**  

---

## Visualizations  
Multiple visuals were created to reveal trends and relationships:  

| Visualization | Description |
|----------------|-------------|
| **Average Inflation by Month** | Shows seasonal inflation trends |
| **Average Yearly Inflation** | Annual inflation comparison |
| **Inflation Heatmap (Year × Month)** | Highlights inflation intensity over time |
| **Correlation Heatmap** | Displays correlation between inflation and other economic variables |
| **Inflation vs. Crude Oil Price** | Dual-axis trend comparison |
| **Year-over-Year Inflation Change (%)** | Highlights percentage fluctuations by year |
| **Inflation Rate Distribution (Histogram)** | Shows spread and variability |
| **CPI Components Composition** | Breakdown of inflation by category |

> All visuals are generated within the notebook but also exported as images in the `visuals/` folder.
