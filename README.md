## 📛 Badges

<p align="left">
  <img alt="Project Status" src="https://img.shields.io/badge/status-completed-brightgreen?style=for-the-badge">
  <img alt="Python" src="https://img.shields.io/badge/Made%20with-Python-3776AB?style=for-the-badge&logo=python&logoColor=white">
  <img alt="License" src="https://img.shields.io/badge/license-MIT-yellow?style=for-the-badge">
  <img alt="Report" src="https://img.shields.io/badge/report-PDF-orange?style=for-the-badge">
  <img alt="Last Updated" src="https://img.shields.io/badge/updated-2025-blue?style=for-the-badge">
  <img alt="Dataset" src="https://img.shields.io/badge/data-PSID-red?style=for-the-badge">
</p>

# 📊 PSID Income Analysis (2001–2023)

This project analyzes how different personal characteristics—such as **military service**, **education**, **age**, and **home ownership**—relate to **family income** over a 22-year period using data from the **Panel Study of Income Dynamics (PSID)**.

The primary goal is to understand **which factors matter most** in predicting income and how their influence changed between **2001** and **2023**.

---

## 📁 Project Overview

The **PSID** is a long-term longitudinal study (running since 1968).  
For this analysis, two cross-sections were extracted:

- **2001** (n = 2,888)
- **2023** (n = 4,428)

The analysis focuses on:

- Simple regressions  
- Multiple regression models  
- Group comparisons (education × military service)  
- Income distribution comparisons over time  

Key variables used:

- Military service  
- College degree completion  
- Age  
- Home ownership  
- Additional demographic controls

---

## 🧹 Data Cleaning

Data cleaning was performed in **Python**, using:

- `pandas` for filtering and restructuring  
- Dropping missing values  
- Renaming PSID variables to readable labels  
- Creating separate dataframes for 2001 and 2023  

After cleaning:

- **2001:** 2,888 valid observations  
- **2023:** 4,428 valid observations  

This produced clean and comparable datasets for modeling.

---

## 📈 Analyses Performed

### 1. **Simple Regression: Military Service → Income**

**2001:** +$9,507 income difference  
**2023:** +$7,604 income difference  

**Interpretation:**  
Military service still has a positive effect on income, but the advantage has decreased by ~20% over time.

---

### 2. **Simple Regression: College Degree → Income**

**2001:** +$34,581 income premium  
**2023:** +$65,246 income premium  

**Interpretation:**  
The college income premium **nearly doubled (+88%)**, showing a rising importance of education.

---

### 3. **Multiple Regression (All Predictors)**

Models included age, military service, college degree, home ownership, and more.

Findings:

- Low R² → demographic characteristics alone **do not strongly predict income**
- Education became a stronger variable over time  
- Military service remained positive but less influential  
- Age shifted from a small positive effect → negative effect  
- Home ownership gained importance  

Income is influenced by many factors beyond simple demographics.

---

### 4. **Combined Group Comparison**

Groups:

1. Military + College  
2. Military + No College  
3. No Military + College  
4. No Military + No College  

Results:

- **Highest incomes:** Military + College  
- **Lowest incomes:** No College + No Military  
- **Largest growth 2001 → 2023:** College groups  

---

## 🖼️ Graphs & Visuals

Add your Python-generated plots in these locations:

- **Income distribution across years** → after “Overview of the Data”
- **Military vs. Non-Military comparison** → after Section 4.1  
- **College vs. No-College comparison** → after Section 4.2  
- **Four-group comparison** → after Section 5  

(Common Python libraries used: `matplotlib`, `seaborn`)

---

## 🧠 Key Conclusions

1. **Education matters far more today than 20 years ago.**  
2. **Military service still helps, but less than before.**  
3. **Multiple regression suggests income is driven by many factors not in simple demographics.**  
4. **The economic landscape has changed:** education has become a stronger indicator of income over time.

---

## 🛠️ Technologies Used (Python)

- **Python 3.x**
- **Libraries:**
  - `pandas`
  - `numpy`
  - `matplotlib`
  - `seaborn`
  - `statsmodels` (or `sklearn`) for regression
- **Environment:** Jupyter Notebook / VS Code
- **Exported Report:** PDF

---

## 📄 Report

The full PDF version of this analysis is included:

`PSID_Data_Analysis_Report.pdf`

---

## 👤 Author

**Julian Izquierdo Martinez**  

