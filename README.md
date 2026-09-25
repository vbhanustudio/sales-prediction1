# Sales Prediction Project
<img src="https://neilpatel.com/wp-content/uploads/2021/02/sales-forecast-3-1200x675.png">
A Machine Learning project using Simple Linear Regression to predict product sales based on advertising platform expenditures, built on the classic ISLR Advertising dataset.

## Table of Contents
- [Project Overview](#project-overview)
- [Dataset Summary](#dataset-summary)
- [Exploratory Data Analysis](#exploratory-data-analysis)
- [Model Architecture](#model-architecture)
- [Installation & Setup](#installation--setup)
- [Usage](#usage)
- [Dependencies](#dependencies)

---

## Project Overview

The objective of this project is to analyze the relationship between media advertising budgets (TV, Radio, Newspaper) and target Sales. Using a Simple Linear Regression framework, we quantify the impact of primary marketing channels—specifically focusing on TV advertising as the primary predictor—to enable data-driven budget allocation.

Key Workflow Steps:
1. **Data Ingestion & Verification**: Loading and inspecting the structure of the advertising dataset.
2. **Data Cleaning**: Outlier detection and missing value auditing.
3. **Exploratory Data Analysis (EDA)**: Visualizing feature distributions and bivariate relationships with target variables.
4. **Model Development**: Training a Linear Regression baseline model.

---

## Dataset Summary

The dataset originates from the *Introduction to Statistical Learning with Applications in R* (ISLR) collection. It consists of 200 records detailing budget allocations (in thousands of dollars) across three media channels alongside the resulting sales (in thousands of units).

| Feature | Data Type | Null Count | Description |
| :--- | :--- | :--- | :--- |
| **TV** | `float64` | 0 Non-Null | Advertising budget spent on TV (in $1,000s) |
| **Radio** | `float64` | 0 Non-Null | Advertising budget spent on Radio (in $1,000s) |
| **Newspaper** | `float64` | 0 Non-Null | Advertising budget spent on Newspaper (in $1,000s) |
| **Sales** *(Target)* | `float64` | 0 Non-Null | Sales of the product (in 1,000 units) |

### Statistical Overview

```text
               TV       Radio   Newspaper       Sales
count  200.000000  200.000000  200.000000  200.000000
mean   147.042500   23.264000   30.554000   15.130500
std     85.854236   14.846809   21.778621    5.283892
min      0.700000    0.000000    0.300000    1.600000
25%     74.375000    9.975000   12.750000   11.000000
50%    149.750000   22.900000   25.750000   16.000000
75%    218.825000   36.525000   45.100000   19.050000
max    296.400000   49.600000  114.000000   27.000000# sales-prediction1
