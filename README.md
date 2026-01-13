# Cardiovascular-Risk-Assessment
hybrid Machine Learning system for heart disease risk prediction with safety constraints.
# Responsible & Interactive Cardiovascular Risk Assessment

A decision support system that integrates a **calibrated Gradient Boosting classifier** with a safety layer based on medical literature.

## 📊 Project Results
This model was trained on 70,000 records to predict heart disease risk.

* **Best Model**: Gradient Boosting
* **Accuracy**: 73.6%
* **ROC-AUC**: 0.802
* **Fairness**: Negligible Equalized Odds Gap of 0.010 across gender

## 🛡️ Key Innovation: Hybrid Safety Architecture
Standard AI models can sometimes suggest harmful correlations (e.g., that smoking reduces risk) due to data noise. This project features a **Safety Override** layer that intercepts erroneous AI advice and replaces it with established medical facts.

## 🛠️ Interactive Tool
The project includes a "Smart Advisor" that doesn't just give a risk score, but calculates the **minimal effective dose** of lifestyle change—such as the exact weight loss needed—to move a patient into a lower risk category.
