## Badges

<p align="left">
  <img alt="Project Status" src="https://img.shields.io/badge/status-completed-brightgreen?style=for-the-badge">
  <img alt="R Language" src="https://img.shields.io/badge/Made%20with-R-276DC3?style=for-the-badge&logo=r&logoColor=white">
  <img alt="License" src="https://img.shields.io/badge/license-MIT-yellow?style=for-the-badge">
  <img alt="Report" src="https://img.shields.io/badge/report-PDF-orange?style=for-the-badge">
  <img alt="Last Updated" src="https://img.shields.io/badge/updated-2025-blue?style=for-the-badge">
  <img alt="Dataset" src="https://img.shields.io/badge/data-PSID-red?style=for-the-badge">
</p>

# PSID Income Analysis (2001–2023)

This project analyzes how different personal characteristics—such as **military service**, **education**, **age**, and **home ownership**—relate to **family income** over a 22-year span using data from the **Panel Study of Income Dynamics (PSID)**.

The core goal is to understand **which factors matter most** in predicting income and how their influence has changed between **2001** and **2023**.

---

## Project Overview

The **PSID** is one of the longest-running household surveys in the world (started in 1968).  
For this project, data from two specific years were cleaned and analyzed:

- **2001** (n = 2,888)
- **2023** (n = 4,428)

The analysis focuses on simple regressions, multiple regression models, and comparisons between demographic groups.

The key variables analyzed include:

- **Military Service** (ever served or not)
- **College Degree** (completed a 4-year degree or not)
- **Age**
- **Home Ownership**
- **Other demographic and household predictors**

---

## Data Cleaning

Data preparation included:

1. Selecting relevant variables  
2. Renaming columns for clarity  
3. Removing missing values  
4. Creating separate datasets for 2001 and 2023  

This ensured a clean structure suitable for regression and visualization.

---

## Analyses Performed

### 1. **Simple Linear Regression: Military Service → Income**
- **2001:** +$9,507 more income for people with military service  
- **2023:** +$7,604 advantage  
- **Trend:** Military impact **declined ~20%** over time  

### 2. **Simple Linear Regression: College Degree → Income**
- **2001:** +$34,581 income premium  
- **2023:** +$65,246 income premium  
- **Trend:** College degree importance **almost doubled (+88%)**

### 3. **Multiple Regression (All Predictors Combined)**
- R² was low in both years → demographic factors alone **do not strongly predict income**
- College degree became a stronger predictor over time  
- Military service remained positive but smaller  
- Age’s effect shifted direction  
- Home ownership became more influential  

### 4. **Group Comparison**
Four combined categories were compared:

1. Military + College  
2. Military + No College  
3. No Military + College  
4. No Military + No College  

**Results:**

- Highest incomes = **College + Military**  
- Lowest incomes = **No College + No Military**  
- Biggest growth from 2001→2023 occurred in **college-educated groups**

---

## Graphs & Visuals

Add your plots in the following places:

- **Income distribution across years** → after “Overview of the Data”
- **Military vs. Non-Military comparisons** → after Section 4.1  
- **College vs. Non-College comparisons** → after Section 4.2  
- **Four-group comparison** → after Section 5  

---

## Key Conclusions

1. **Education matters more today than 20 years ago**  
   The income gap for college graduates nearly doubled.

2. **Military service still helps—but less**  
   The income advantage shrank over time.

3. **Demographics alone cannot explain income differences**  
   Even with several variables, models had low explanatory power.

4. **The world has changed**  
   Education’s importance increased sharply, while military benefits in the labor market weakened.

---

## Technologies Used

- **Python** (Data cleaning, regression, visualization)
- Libraries: `tidyverse`, `dplyr`, `ggplot2`, `readr`
- Methods: simple linear regression & multiple regression

