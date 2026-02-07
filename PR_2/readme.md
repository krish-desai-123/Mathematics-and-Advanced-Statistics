# 📊 Expectation Decider: Statistical Inference on Student Success

[![Python](https://img.shields.io/badge/Python-3.8%2B-blue?logo=python&logoColor=white)](https://www.python.org/)
[![Pandas](https://img.shields.io/badge/Library-Pandas-150458?logo=pandas)](https://pandas.pydata.org/)
[![Stats](https://img.shields.io/badge/Field-Probability%20%26%20Statistics-orange)](#)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)

> **Predicting academic outcomes through the lens of Bayesian Theory and Probability Distributions.**

**Expectation Decider** is a comprehensive data analysis project that bridges the gap between raw student data and mathematical certainty. By applying core statistical concepts like **Bayes' Theorem**, **Conditional Probability**, and **Random Variable Distributions**, this project identifies the hidden patterns that lead to academic success.

---

## 🌟 Project Highlights

- **Data-Driven Insights**: Analyzes 200+ student records to quantify the impact of study habits and attendance.
- **Probabilistic Modeling**: Implements theoretical vs. empirical comparisons for performance prediction.
- **Bayesian Inference**: Uses conditional logic to determine the real-world probability of passing exams based on behavioral triggers.
- **Visual Analytics**: Features Venn diagrams and contingency tables to visualize dependencies between variables.

---

## 📂 Dataset Architecture

The analysis is performed on `expectation_decider_dataset.csv`, featuring a multidimensional view of student behavior:

| Column | Type | Description |
| :--- | :--- | :--- |
| `study_hours` | *Numerical* | Weekly hours dedicated to self-study. |
| `attendance` | *Numerical* | Percentage of classes attended. |
| `group_discussion` | *Categorical* | Involvement in collaborative study groups (Yes/No). |
| `previous_test_score`| *Numerical* | Performance in baseline assessments. |
| **`final_exam_pass`** | **Target** | The binary outcome: **Pass** or **Fail**. |

---

## 🧠 The Mathematics of Success

### 1. Empirical vs. Theoretical Probability
We compare the observed frequency of passing ($P_{empirical}$) against a balanced theoretical model ($P = 0.5$) to identify performance biases in the student cohort.

### 2. Random Variables & Distribution
Modeling the success of a subset (e.g., 3 students) as a discrete random variable $X$:
- **Expected Value**: $E[X] = \sum x \cdot P(x) = 1.5$
- **Variance**: $Var(X) = E[X^2] - (E[X])^2 = 0.625$

### 3. Bayesian Logic (The Core)
The project calculates the posterior probability of passing given high attendance using **Bayes’ Theorem**:

$$P(Pass | High Attendance) = \frac{P(High Attendance | Pass) \cdot P(Pass)}{P(High Attendance)}$$

**Key Result:** In this dataset, students with high attendance (>80%) saw their probability of passing surge to approximately **89%**, proving that attendance is a critical predictor of success.

---

## 📊 Visual Analysis

### 📈 Contingency Tables
By cross-tabulating `group_discussion` and `final_exam_pass`, the project reveals a strong dependency:
- **Observation**: Participation in group discussions acts as a catalyst, significantly shifting the marginal probability of passing.

### ⭕ Venn Diagrams
Visualizes the intersection of two critical success factors:
- **Set A**: Students studying $> 10$ hours/week.
- **Set B**: Students with $> 80\%$ attendance.
- **Outcome**: Identifying the "Gold Zone" where both conditions meet.

---

## 🚀 How to Run
1. Open the notebook: `expectation_decider.ipynb`.
2. Ensure `expectation_decider_dataset.csv` is in the same directory.
3. Run all cells to generate the statistical reports and visualizations.

---

## 💡 Key Conclusion
The project concludes that academic success is not random. Through **Bayesian Inference**, we demonstrate that specific behaviors—primarily high attendance and group participation—shift the "Expectation" from a coin-flip (50/50) to a statistically significant certainty.

---

**Developed with ❤️ by Krish Desai** *Exploring the intersection of Data Science and Statistics.*