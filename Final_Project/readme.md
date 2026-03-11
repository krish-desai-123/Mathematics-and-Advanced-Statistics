# 📊 Mathematics & Advanced Statistics Analysis

[![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)](https://python.org)
[![Jupyter](https://img.shields.io/badge/Jupyter-F37626?style=for-the-badge&logo=Jupyter&logoColor=white)](https://jupyter.org)
[![Pandas](https://img.shields.io/badge/Pandas-150458?style=for-the-badge&logo=pandas&logoColor=white)](https://pandas.pydata.org/)
[![NumPy](https://img.shields.io/badge/NumPy-013243?style=for-the-badge&logo=numpy&logoColor=white)](https://numpy.org/)

> **A comprehensive exploratory data analysis (EDA) and statistical modeling project exploring student performance metrics through probability, variance, and linear algebra.**

---

## 🚀 Project Overview

This repository contains a full-stack data science notebook designed to extract actionable insights from student academic data. By applying foundational mathematics and advanced statistical concepts, this project evaluates the correlation between study habits and passing rates while plotting the distributions of various test scores. 

## 📂 Repository Structure

* 📓 **`final_project.ipynb`** - The core Jupyter Notebook containing all Python code, data wrangling, and visualizations.
* 📄 **`students_scores.csv`** - The dataset featuring 4,950+ student records (ID, Age, Math/Science/English Scores, Hours Studied, and Pass/Fail status).
* 📕 **`final_project.pdf`** - Theoretical documentation covering short questions on the underlying math (Normal Distribution, Bayes Theorem, Skewness, Kurtosis, Eigenvalues, etc.).

---

## ✨ Key Features & Methodologies

### 📈 1. Descriptive Statistics
Calculates central tendencies and dispersion metrics for student scores using Pandas and NumPy:
* **Mean, Median, & Mode** for Math scores.
* **Range, Variance, & Standard Deviation** for Science scores.

### 🎲 2. Probability & Hypothesis
Evaluates academic success based on time investment:
* Generates a **Contingency Table** mapping `Pass/Fail` against `Hours Studied > 5`.
* Calculates the conditional probability of passing given a specific study threshold.

### 📐 3. Linear Algebra & Vectors
Applies core mathematical operations using NumPy:
* Computes **L1 & L2 Norms**.
* Calculates the **Dot Product** and the exact **Angle between vectors** (in degrees and radians) to analyze score relationships.

### 📊 4. Data Visualization
* Utilizes **Seaborn** and **Matplotlib** to map out KDE-enabled histograms, showcasing the probability density and normal distribution curve of the Math scores.

---

## 🛠️ Tech Stack & Libraries

This project relies on the following standard Data Science and Software Engineering libraries:
* **Python** 🐍
* **Pandas** 🐼 - For data manipulation and reading the CSV.
* **NumPy** 🔢 - For linear algebra and vector math.
* **Seaborn & Matplotlib** 📉 - For aesthetic and statistical data visualization.
* **SciPy (stats)** 🔬 - For advanced statistical modeling.

---

## 💡 Learnings & Takeaways

This project serves as a practical bridge between theoretical mathematics and applied software engineering. From calculating empirical probabilities to handling vector spaces in Python, it demonstrates a strong foundational grasp of the math required for modern Data Science.

---

<div align="center">
  <i>Built with ☕ and Python</i>
</div>