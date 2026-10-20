# Healthcare Data Analysis & Insights

This repository provides a comprehensive end-to-end Exploratory Data Analysis (EDA) on a healthcare dataset containing patient records. The objective of this project is to clean, analyze, and visualize various patient demographics, medical conditions, billing metrics, and admission patterns to 
# Healthcare Data Analysis & Insights

This repository provides a comprehensive end-to-end Exploratory Data Analysis (EDA) on a healthcare dataset containing patient records. The objective of this project is to clean, analyze, and visualize various patient demographics, medical conditions, billing metrics, and admission patterns to uncover key operational and clinical insights.

---

## Table of Contents
- [Dataset Overview](#dataset-overview)
- [Data Preprocessing](#data-preprocessing)
- [Key Analysis & Questions Answered](#key-analysis--questions-answered)
- [Major Findings](#major-findings)
- [Technologies Used](#technologies-used)
- [How to Run the Notebook](#how-to-run-the-notebook)

---

## Dataset Overview

The dataset consists of **55,500 initial records** with 15 detailed feature columns representing clinical and financial logs:

*   **Demographics:** Name, Age, Gender, Blood Type
*   **Clinical Data:** Medical Condition, Doctor, Hospital, Admission Type, Date of Admission, Discharge Date, Medication, Test Results
*   **Financial & Logistical Data:** Billing Amount, Room Number, Duration of Stay (Derived)

---

## Data Preprocessing

1.  **Duplicate Removal:** Identified and dropped **534 duplicate records** to ensure data integrity, reducing the dataset size to **54,966 unique observations**.
2.  **Date Conversion:** Converted `Date of Admission` and `Discharge Date` columns to datetime objects.
3.  **Feature Engineering:** Engineered a new column `Duration of stay (Days)` to measure the total hospital duration for each patient.
4.  **Anomaly Detection:** Discovered and isolated **106 entries** with negative `Billing Amount` values for separate accounting validation.

---

## Key Analysis & Questions Answered

The Jupyter notebook addresses several critical operational and medical questions:

1.  **Test Results Status:** Calculated percentages of Normal, Abnormal, and Inconclusive results.
2.  **Age Demographics:** Visualized the age distribution of patients via histograms.
3.  **Gender Split:** Verified the overall balance between male and female admissions.
4.  **Blood Type Distribution:** Counted and charted occurrences of each blood type group.
5.  **Gender Distribution across Blood Types:** Cross-tabulated gender representation for different blood groups.
6.  **Medical Conditions Prevalence:** Visualized the volume distribution of various chronic diseases (e.g., Arthritis, Diabetes, Obesity).
7.  **Disease Impact by Gender:** Evaluated if specific medical conditions preferentially impact a certain gender.
8.  **Patient Segmentations:** Analyzed patients broken down by sex, medical condition, and blood type.
9.  **Medication Distribution:** Analyzed prescription frequencies for drugs like Lipitor, Ibuprofen, Aspirin, and others.
10. **Medication vs. Condition Mapping:** Mapped what medical conditions are associated with which prescribed drug.
11. **Admission Type Analysis:** Segmented admissions (Elective, Emergency, Urgent) across genders and prescribed medications.
12. **Financial Outliers:** Located the maximum and minimum billing amounts, identifying patients with negative balances.
13. **Operational Metrics:** Identified long-stay patients (max 30 days) and short-stay patients (min 1 day).

---

## Major Findings

*   **Demographics:** The cohort shows an extremely balanced representation between Genders (50.02% Male vs. 49.98% Female).
*   **Test Outcome Consistency:** Test results are nearly equally divided into Abnormal (33.5%), Normal (33.3%), and Inconclusive (33.1%).
*   **Financials:** The average billing amount hovers around **$25,544.30** with a maximum billing outlier at **$52,764.28** and anomalous negative charges down to **-$2,008.49**.
*   **Hospital Stays:** Hospital stay durations are evenly spread across the dataset, ranging from a minimum of **1 day** up to a maximum limit of **30 days**.

---

## Technologies Used

*   **Python 3.x**
*   **Pandas** - Data manipulation and analysis
*   **NumPy** - Numerical computing
*   **Matplotlib** - Static visualizations
*   **Seaborn** - Statistical data visualization
