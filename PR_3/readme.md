# 🏥 Derivable Judgement: Health & Lifestyle Statistical Analysis

![Python](https://img.shields.io/badge/Python-3.8%2B-blue?style=for-the-badge&logo=python&logoColor=white)
![Jupyter](https://img.shields.io/badge/Jupyter-Notebook-orange?style=for-the-badge&logo=jupyter&logoColor=white)
![Pandas](https://img.shields.io/badge/Pandas-Data%20Analysis-150458?style=for-the-badge&logo=pandas&logoColor=white)
![Status](https://img.shields.io/badge/Status-Completed-success?style=for-the-badge)

> **"Data is the new oil, but statistical analysis is the refinery."**

## 📖 Overview

This project performs a comprehensive **Inferential Statistical Analysis** on a healthcare dataset. The goal is to derive meaningful judgements about how lifestyle choices (like smoking) and demographic factors (like age and gender) impact critical health metrics such as **BMI**, **Glucose Levels**, and **Diabetes** prevalence.

By applying rigorous statistical tests—including **Z-tests, Chi-Square, ANOVA, and Spearman Correlation**—this project moves beyond simple observation to prove statistical significance in health trends.

---

## 📂 Dataset Description

The analysis is based on `derivable_judgement_dataset.csv`, containing health records for various patients.

| Column Name | Data Type | Description |
| :--- | :--- | :--- |
| **Age** | `Numeric` | Age of the patient in years. |
| **Gender** | `Categorical` | Male or Female. |
| **Weight** | `Numeric` | Weight in kilograms (kg). |
| **BMI** | `Numeric` | Body Mass Index. |
| **Blood Pressure** | `Numeric` | Systolic blood pressure reading. |
| **Cholesterol** | `Numeric` | Cholesterol levels (mg/dL). |
| **Glucose** | `Numeric` | Blood glucose levels. |
| **Smoking Status** | `Categorical` | Smoker or Non-Smoker. |
| **Diabetes** | `Categorical` | Yes or No (Diabetes diagnosis). |

---

## ⚙️ Methodology & Statistical Tests

We utilized a structured statistical approach to validate our hypotheses:

### 1️⃣ Data Cleaning & Preprocessing
* Handling missing values and data type conversion.
* Categorizing continuous variables (e.g., creating `Age Groups`).

### 2️⃣ Hypothesis Testing (The Core)
We applied the following tests to answer key medical questions:

| Statistical Test | Question Answered |
| :--- | :--- |
| **Z-Test (Two-Sample)** | Do **Smokers** have significantly different health metrics (BP, Glucose) than **Non-Smokers**? |
| **Chi-Square Test** | Is there a dependency between **Smoking Status** and **Diabetes**? |
| **One-Way ANOVA** | Does **BMI** vary significantly across different **Age Groups**? |
| **Spearman Correlation** | Is there a monotonic relationship between **Age** and **BMI**? |

---

## 📉 Key Findings & Derivable Judgements

Based on the statistical output, here are the derived insights:

### 🚬 Impact of Smoking
* **Glucose & BP:** The Z-test analysis revealed that smokers have significantly higher glucose and blood pressure levels compared to non-smokers ($p < 0.05$).
* **Diabetes Link:** The Chi-Square test confirmed a statistically significant dependency between **Smoking** and **Diabetes Prevalence** (Reject $H_0$).

### ⚖️ Age & BMI Dynamics
* **Age Groups:** The ANOVA test showed that BMI is **not constant** across life stages; there is a significant variance in BMI between different age groups.
* **Correlation:** Spearman's rank correlation indicated a moderate positive trend, suggesting BMI tends to change as age increases.

---

## 📊 Visualizations

The notebook includes professional visualizations to support the statistical findings:
* 🔥 **Correlation Heatmap:** To visualize relationships between all numerical variables.
* 📦 **Boxplots:** To display BMI distribution across Age Groups (ANOVA visualization).
* 📊 **Countplots:** To show the frequency of Diabetes among Smokers vs. Non-Smokers.

---

## 🛠️ Tech Stack

* **Language:** Python 🐍
* **Environment:** Jupyter Notebook 📓
* **Libraries:**
    * `pandas` & `numpy` (Data Manipulation)
    * `scipy.stats` (Statistical Testing)

---

## 👨‍💻 Author

**Krish Desai**
* Data Analyst & Python Developer

---

*This project is for educational and analytical purposes.*