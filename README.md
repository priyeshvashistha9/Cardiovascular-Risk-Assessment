# Responsible & Interactive Cardiovascular Risk Assessment
### A Hybrid Machine Learning Approach with Safety Constraints

This project presents an interactive decision support system for predicting cardiovascular risk. It combines a high-performing Gradient Boosting model with a Hybrid Safety Architecture to ensure health advice remains clinically valid.

---

## 🚀 Key Features
* **Predictive Power:** Achieves an ROC-AUC of 0.802 and 73.6% accuracy.
* **Hybrid Safety Layer:** A logic system that overrides AI predictions if they contradict medical facts.
* **Responsible AI Audit:** Verified for fairness with a negligible gender bias gap (< 0.01).
* **Interactive Smart Advisor:** A tool that calculates the weight loss required to lower patient risk.

---

## 📊 Performance Summary
| Model | Accuracy | ROC-AUC |
| :--- | :--- | :--- |
| Logistic Regression | 72.7% | 0.791 |
| Random Forest | 73.3% | 0.801 |
| **Gradient Boosting (Final)** | **73.6%** | **0.802** |

---

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
