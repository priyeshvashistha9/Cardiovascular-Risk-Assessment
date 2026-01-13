# Responsible & Interactive Cardiovascular Risk Assessment
### A Hybrid Machine Learning Approach with Safety Constraints

This project presents an interactive decision support system for predicting cardiovascular risk. It uniquely combines a high-performing **Gradient Boosting** model with a **Hybrid Safety Architecture** to ensure that all health advice remains clinically valid and responsible.

---

## 🚀 Key Features
* **Predictive Power:** Achieves an **ROC-AUC of 0.802** and **73.6% accuracy**.
* **Hybrid Safety Layer:** A built-in logic system that overrides AI predictions if they contradict medical facts (e.g., ensuring smoking is never flagged as "healthy").
* **Responsible AI Audit:** Verified for fairness with a negligible gender bias gap (< 0.01).
* **Interactive Smart Advisor:** Includes a tool that calculates the "minimal effective dose" of lifestyle change, such as exact weight loss required to lower risk.

---

## 📊 Model Performance
After comparing multiple algorithms, the Gradient Boosting model was selected for its superior calibration and accuracy:

| Model | Accuracy | ROC-AUC |
| :--- | :--- | :--- |
| Logistic Regression | 72.7% | 0.791 |
| Random Forest | 73.3% | 0.801 |
| **Gradient Boosting (Final)** | **73.6%** | **0.802** |

---

## 🛠 Installation & Usage
To run this project on your local machine, follow these steps:

1. **Install Dependencies:**
   Open your terminal/command prompt and run:
   ```bash
   pip install pandas scikit-learn matplotlib numpy
