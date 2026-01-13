# Responsible & Interactive Cardiovascular Risk Assessment
### A Hybrid Machine Learning Approach with Safety Constraints

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![Python 3.8+](https://img.shields.io/badge/python-3.8+-blue.svg)](https://www.python.org/downloads/)

## 📖 Project Overview
Cardiovascular disease is a leading cause of global mortality. While Machine Learning (ML) offers powerful predictive capabilities, standard "black-box" models often lack the safety mechanisms—interpretability, fairness, and clinical grounding—required for healthcare deployment.

This project introduces a **Hybrid Safety Architecture**. It integrates a high-performing Gradient Boosting classifier with a deterministic "Safety Layer" based on established medical literature. This ensures the system never provides counter-intuitive advice (e.g., suggesting that increasing blood pressure reduces risk) due to data noise.

<p align="center">
  <img src="interface.png" width="45%" />
  <img src="results.png" width="45%" />
</p>


## 🚀 Technical Features & Methodology
* **Data Engineering:** Conducted an ablation study on pre-processing, specifically targeting outliers in Systolic/Diastolic blood pressure and BMI calculations to improve model stability.
* **Multi-Model Benchmarking:** Evaluated Logistic Regression, Random Forest, and Gradient Boosting.
* **Probability Calibration:** Applied **Sigmoid Calibration** to ensure that predicted risk scores represent real-world empirical probabilities.
* **Hybrid Safety Override:** A hard-coded medical logic layer that intercepts AI predictions. If the AI suggests a lifestyle change that contradicts medical science, the Safety Layer overrides the output with clinically sound advice.
* **Responsible AI Audit:** The system was audited for demographic fairness, achieving a negligible **Equalized Odds Gap of 0.010**, ensuring no systematic bias against gender groups.

## 📊 Performance Summary
| Metric | Logistic Regression | Random Forest | **Gradient Boosting (Final)** |
| :--- | :--- | :--- | :--- |
| **Accuracy** | 72.7% | 73.3% | **73.6%** |
| **ROC-AUC** | 0.791 | 0.801 | **0.802** |

 **Gender Fairness (Equalized Odds Gap)** | < 0.010 

## 🛠️ Installation & Usage
To run this project on your local machine:

1. **Install Dependencies:**
   Run this command in your terminal:
   `pip install pandas scikit-learn matplotlib numpy`

2. **Run the Notebook:**
   Open `872.ipynb` in Jupyter Notebook or upload it to Google Colab.

3. **Data Requirements:**
   Ensure `cardio_train.csv` is in the same folder as the notebook.

---

## 📂 Project Structure
* **872.ipynb**: Full source code and interactive tool.
* **priyesh-872-finalReport.pdf**: Detailed research paper.
* **cardio_train.csv**: Dataset (70,000 records).

---

## 🎓 Author & Credits
**Author:** Priyesh Vashistha  
**Institution:** Department of Electrical and Computer Engineering, Queen's University  
**Data Source:** Cardiovascular Disease Dataset from Kaggle  

---
**Disclaimer:** This tool is for educational purposes only and is not a substitute for professional medical advice.
