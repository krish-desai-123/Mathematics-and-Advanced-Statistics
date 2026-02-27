# 📊 Spread Locator: E-Commerce Statistical Distribution Analysis

![Python](https://img.shields.io/badge/Python-3.8%2B-blue?style=for-the-badge&logo=python&logoColor=white)
![Jupyter](https://img.shields.io/badge/Jupyter-Notebook-orange?style=for-the-badge&logo=jupyter&logoColor=white)
![SciPy](https://img.shields.io/badge/SciPy-Statistical%20Analysis-darkblue?style=for-the-badge&logo=scipy&logoColor=white)
![Status](https://img.shields.io/badge/Status-Completed-success?style=for-the-badge)

> **"Distributions are the hidden fingerprints of data behaviors."**

## 📖 Overview

This project performs a comprehensive **Statistical Distribution Analysis** on an e-commerce transaction dataset. The goal is to understand customer purchase behaviors, effectively handle highly skewed financial data, and derive actionable probability insights.

By applying rigorous statistical modeling—including **Distribution Fitting (Log-Normal, Poisson, Bernoulli), Q-Q Plots, Box-Cox Transformations, and Z-Score Probabilities**—this project moves beyond simple descriptive statistics to uncover the true mathematical "spread" of the data.

---

## 📂 Dataset Description

The analysis is based on `spread_locator_dataset.csv`, containing daily transaction records for e-commerce customers.

| Column Name | Data Type | Description |
| :--- | :--- | :--- |
| **transaction_id** | `UUID/String` | Unique identifier for each transaction. |
| **customer_id** | `UUID/String` | Unique identifier for each customer. |
| **transaction_amount** | `Float` | Total amount of the transaction. |
| **transaction_date** | `Date` | Date the transaction occurred. |
| **transaction_count** | `Int` | Number of transactions made by a customer in a given week. |
| **region** | `String` | Customer's geographic region (North, South, East, West). |
| **transaction_status** | `String` | Whether the transaction was successful (Success/Fail). |

---

## ⚙️ Methodology & Statistical Modeling

We utilized a structured statistical approach to fit, test, and transform the data:

### 1️⃣ Data Preparation
* Parsing dates, handling data types, and isolating continuous vs. discrete variables.

### 2️⃣ Statistical Testing (The Core)
We applied the following methods to answer key business and statistical questions:

| Statistical Concept | Application / Question Answered |
| :--- | :--- |
| **Discrete Distributions** | Fitting **Bernoulli** (Success/Fail rates) and **Binomial** (Weekly transaction counts). |
| **Poisson Distribution** | Modeling the average rate of transactions occurring per day. |
| **Continuous Distributions** | Fitting **Log-Normal** and **Power Law** models to transaction amounts. |
| **Q-Q Plot** | Visually testing if transaction amounts strictly follow a Normal Distribution. |
| **Box-Cox Transform** | Stabilizing variance and normalizing heavily skewed, non-negative financial data. |
| **Z-Score Probability** | Computing the exact probability of high-value, extreme transactions (e.g., > 5000). |

---

## 📉 Key Findings & Derivable Insights

Based on the statistical output, here are the derived judgements:

### ⚖️ Skewness & Normality
* **Not Normal:** The Q-Q plot analysis confirmed that raw transaction amounts are highly right-skewed and significantly deviate from a standard normal distribution. 
* **Variance Stabilization:** The **Box-Cox transformation** successfully stabilized the variance. The optimal lambda ($\lambda$) value indicated that a logarithmic transformation is highly effective for normalizing this specific financial dataset.

### 📈 Best Fit Models
* **Transaction Amounts:** Due to the non-negative nature of the data and the long tail of high-value purchases, the **Log-Normal Distribution** provided the most accurate continuous fit for predicting transaction amounts.
* **Daily Frequency:** The **Poisson distribution** accurately modeled the frequency of daily transactions, establishing a reliable expected mean ($\lambda$).

### 🎯 Predictive Probabilities
* **High-Value Predictions:** Z-score standardizations allowed us to calculate the theoretical probability of transactions exceeding 5000, establishing a baseline for anomaly detection and financial forecasting.

---

## 📊 Visualizations

The notebook includes professional visualizations to support the mathematical findings:
* 📉 **Q-Q Plots:** To visually diagnose deviations from theoretical normality at the quantiles.
* 📊 **PDF & CDF Plots:** Kernel Density Estimates (PDF) and Empirical Cumulative Distribution (CDF) charts to showcase the distribution of transaction amounts.
* 📦 **Transformation Overlays:** Visualizing the data shape before and after the Box-Cox transformation.

---

## 🛠️ Tech Stacks

* **Language:** Python 🐍
* **Environment:** Jupyter Notebook 📓
* **Libraries:**
    * `pandas` & `numpy` (Data Manipulation)
    * `scipy.stats` (Advanced Statistical Testing & Fitting)
    * `matplotlib` & `seaborn` (Data Visualization)

---

## 👨‍💻 Author

**Krish Desai**
* Data Analyst & Python Developer

---

*This project is for educational and analytical purposes, focusing on advanced statistics and probability.*