# 📊 Telecom Customer Churn Prediction Pipeline

An end-to-end Machine Learning pipeline built in Python to address a critical business challenge: **Customer Retention**. This project engineers a robust data preprocessing workflow and benchmarks three classification algorithms to identify at-risk customers before they churn.

---

## 🚀 Business Objective & Insights
Customer churn directly impacts revenue. The goal of this project is to maximize **Recall**—identifying the highest percentage of actual churning customers so marketing teams can target them with retention incentives.

### 🏆 The Algorithm Showdown
While complex models are often assumed to be superior, a strict baseline comparison revealed **Logistic Regression** as the optimal choice for this business use case due to its superior sensitivity to capturing positive churn cases.

| Model | Accuracy | Precision | Recall (Catch Rate) |
| :--- | :---: | :---: | :---: |
| **Logistic Regression** 🏆 | **81.97%** | 65.00% | **60.00%** |
| **Support Vector Machine (SVM)** | 81.41% | **69.00%** | 53.00% |
| **k-Nearest Neighbors (k-NN)** | 77.08% | 56.00% | 51.00% |

> **Key Business Takeaway:** Logistic Regression captured **60% of churning customers**—outperforming the complex SVM model by a margin of 7% in Recall. In a real-world scenario, this gap represents significant recovered revenue.

---

## 🛠️ Tech Stack & Features
* **Language:** Python
* **Environment:** Jupyter Notebooks / VS Code
* **Libraries:** Pandas, NumPy, Scikit-Learn, Seaborn, Matplotlib, Kagglehub
* **Data Pipeline Features:**
  * Automated data retrieval using `kagglehub` API.
  * Robust data cleaning (handling invalid types and missing value imputation via medians).
  * Feature encoding using categorical dummy variables.
  * Standard Feature Scaling to guarantee distance-based algorithm performance.

---

## 🏃 How to Run This Project Locally

### 1. Clone the Repository
```bash
git clone [https://github.com/tayyabanaveed358-dev/customer-churn-prediction.git](https://github.com/tayyabanaveed358-dev/customer-churn-prediction.git)
cd customer-churn-prediction