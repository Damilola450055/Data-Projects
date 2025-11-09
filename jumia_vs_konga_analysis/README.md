# Jumia vs Konga iPhone Price Analysis

## Overview

This project analyzes iPhone prices across Jumia and Konga, two of Nigeria’s largest e-commerce platforms.
It focuses on **comparing price trends**, **availability**, and **correlations** between both marketplaces using data scraped directly from their websites.

**Data was collected using standard web scraping methods on publicly available web pages. The process strictly followed ethical scraping guidelines and respected the robots.txt rules of both platforms, ensuring that no security measures were bypassed and no Terms of Service were violated.**

---

## Phase 1 — Web Scraping
**Tools Used**: BeautifulSoup, Requests, Pandas

**Goal**:
Collect iPhone listings (model, price) from Jumia and Konga.

**Process**:
- Scraped multiple pages from both platforms
- Extracted product names and prices

**Saved raw data as**: 
- jumia_iphone.csv
- konga_iphone.csv
  
---

## Phase 2 — Data Cleaning
**Tools Used**: Pandas, re, NumPy

**Steps**:
- Converted all price data to numeric format
- Cleaned price data by removing currency symbols (₦) and commas
- Extracted iPhone series using regex 
- Correct invalid entries

**Saved cleaned files as**:
- cleaned_jumia_iphone.csv
- cleaned_konga_iphone.csv
  
---

## Phase 3 — Data Analysis
**Objectives**:
Understand cross-platform price differences and product distribution.

**Insights**:
- Identified iPhone models unique to each platform
- Found common models available on both Jumia and Konga
- Calculated average, minimum, and maximum prices per series
- Determined most frequently listed iPhone series
- Highlighted phones priced closest to each platform’s average

---

## Phase 4 — Visualization
**Tools Used**: Matplotlib, Seaborn

**Visuals Created**
| Visualization | Description |
|-----------------|--------------|
| **Price Distribution (Boxplot)** | Compares price variability between Jumia and Konga |
| **Average Price Trend (Line Chart)** | Shows pricing pattern by iPhone series |
| **Price Correlation (Scatter + Heatmap)** |	Reveals relationship between prices on both sites |

## Tools & Libraries
- **Python**
  - BeautifulSoup
  - Requests
  - Pandas
  - re
  - NumPy
  - Matplotlib
  - Seaborn
- **Jupyter**
