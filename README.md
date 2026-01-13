# Cardiovascular-Risk-Assessment
hybrid Machine Learning system for heart disease risk prediction with safety constraints.
# Responsible & Interactive Cardiovascular Risk Assessment
### A Hybrid Machine Learning Approach with Safety Constraints

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![Python 3.8+](https://img.shields.io/badge/python-3.8+-blue.svg)](https://www.python.org/downloads/)

## 📖 Project Overview
Cardiovascular disease remains a leading cause of global mortality. While Machine Learning (ML) offers powerful predictive capabilities, standard "black-box" models often lack the safety mechanisms—like interpretability and clinical grounding—required for actual healthcare deployment.

This project introduces a **Hybrid Safety Architecture**. It combines a high-performing Gradient Boosting classifier with a deterministic "Safety Layer" that ensures the AI never gives advice that contradicts established medical literature (e.g., suggesting that smoking or high blood pressure decreases risk).

## 🚀 Key Features
* **Multi-Model Benchmarking:** Comparative analysis of Logistic Regression, Random Forest, and Gradient Boosting.
* **Probability Calibration:** Uses Sigmoid calibration to ensure the risk scores (0–100%) align with real-world empirical probabilities.
* **Safety Override Logic:** A hard-coded medical logic layer that intercepts erroneous AI predictions.
* **Interactive Smart Advisor:** A tool that calculates the "minimal effective dose" of lifestyle change (e.g., "Lose 4kg to move from High Risk to Moderate Risk").
* **Responsible AI Audit:** Evaluated for demographic fairness using the Equalized Odds metric.

## 📊 Performance Summary
After an extensive ablation study on pre-processing (handling outliers in blood pressure and BMI), the **Gradient Boosting** model was selected as the champion:

| Metric | Result |
| :--- | :--- |
| **Accuracy** | 73.6% |
| **ROC-AUC** | 0.802 |
| **Gender Fairness (Equalized Odds Gap)** | < 0.010 |

## 🛡️ Responsible AI & Safety
In healthcare, a model being "accurate" isn't enough; it must be **safe**. 
1. **The Safety Layer:** If the ML model incorrectly predicts that a smoker has lower risk than a non-smoker (due to data noise), our Hybrid Architecture overrides the result to maintain clinical validity.
2. **Fairness:** We conducted a fairness audit to ensure the model performs equally well for all genders, preventing systematic bias in medical leaf-lets.

## 🛠️ Installation & Usage
1. **Clone the repo:**
   ```bash
   git clone [https://github.com/YOUR_USERNAME/YOUR_REPO_NAME.git](https://github.com/YOUR_USERNAME/YOUR_REPO_NAME.git)
