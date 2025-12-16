# Inequality in Education Analysis

## Overview

This project analyzes global **education inequality trends from 2013–2021** using publicly available country-level data. The objective is to understand how education inequality varies across regions and human development groups, and how it relates to broader development indicators such as **Human Development Index (HDI)**.

The project is designed as an **applied data analysis case study**, focusing on data cleaning, exploratory analysis, and quantitative insight generation rather than pure visualization.

---

## Problem Statement

Education inequality remains a persistent global issue, but its relationship with overall human development is not uniform across regions.

This project aims to answer the following questions:

* How does education inequality vary across continents and human development groups?
* What trends can be observed in education inequality from 2013 to 2021?
* How strongly is education inequality associated with HDI rank?

---

## Dataset

* **Source:** Global education inequality and human development indicators
* **Granularity:** Country-level data
* **Time Range:** 2013–2021
* **Key Variables:**

  * Education inequality index (yearly)
  * HDI Rank (2021)
  * Continent
  * Human Development Group

---

## Methodology

### 1. Data Preparation

* Inspected data structure, summary statistics, and missing values
* Removed columns with excessive missing data (2010–2012)
* Handled missing yearly values using forward-filling assumptions within country-level time series
* Normalized education inequality metrics using min-max scaling for comparability across years

### 2. Exploratory Data Analysis (EDA)

* Distribution analysis of education inequality
* Comparison across human development groups and continents
* Temporal trend analysis (2013–2021)
* Correlation analysis between education inequality and HDI rank

### 3. Quantitative Analysis

* Computed correlation matrix for numeric variables
* Analyzed relationship between HDI rank and education inequality using correlation coefficients
* Aggregated inequality metrics by continent to identify regional patterns

### 4. Visualization

* Interactive histograms, scatter plots, and box plots
* Heatmaps to highlight temporal and regional trends
* Choropleth world map to visualize global inequality distribution (2021)

---

## Key Insights

* Countries with lower HDI ranks tend to exhibit higher education inequality, although the relationship is not perfectly linear
* Education inequality shows persistent regional disparities, with certain continents consistently exhibiting higher average inequality
* Middle-development groups show the widest variance, suggesting uneven progress within similar development levels

---

## Tools & Technologies

* **Language:** R
* **Libraries:** tidyverse, ggplot2, plotly, DT, sf, rnaturalearth
* **Techniques:** Data cleaning, normalization, correlation analysis, aggregation, interactive visualization

---

## Project Structure

```
├── data/
│   └── Inequality in Education_2.csv
├── analysis/
│   └── education_inequality_analysis.Rmd
├── output/
│   ├── education_inequality_analysis.html
│   └── education_inequality_analysis.pdf
└── README.md
```

---

## Limitations & Future Work

* The analysis focuses on descriptive and correlational insights; causal relationships are not established
* Missing value handling relies on temporal assumptions that could be refined
* Future extensions may include regression modeling, clustering of countries, or predictive trend analysis

---

## Author

Group project contribution focusing on data preprocessing, exploratory analysis, and visualization.
