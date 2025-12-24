# 🛒 E-commerce Fraud Detection using Machine Learning

## 📌 Project Overview
E-commerce platforms frequently face losses due to fraudulent transactions.  
This project focuses on building a **machine learning–based fraud detection system** to identify suspicious transactions while addressing the challenge of **class imbalance**.

The project emphasizes **proper evaluation metrics** such as precision, recall, and F1-score instead of relying only on accuracy.

---

## 📊 Dataset Description
The dataset contains transaction-level data including user behavior, transaction details, security verification results, and fraud labels.

### Key Features:
- `transaction_id`, `user_id`
- `account_age_days`
- `total_transactions_user`, `avg_amount_user`
- `amount`
- `country`, `bin_country`
- `channel`, `merchant_category`
- `promo_used`
- `avs_match`, `cvv_result`, `three_ds_flag`
- `transaction_time`
- `shipping_distance_km`

**Target Variable:**
- `is_fraud`  
  - 0 → Legitimate Transaction  
  - 1 → Fraudulent Transaction

---

## 🔍 Exploratory Data Analysis (EDA)
EDA was performed to understand fraud patterns and guide model selection.

### Key Insights:
- The dataset is **highly imbalanced**, with fraud cases being a small percentage.
- Fraudulent transactions are more common for **new user accounts**.
- **Promo code usage** shows higher fraud occurrence.
- Failed **AVS/CVV checks** and missing **3-D Secure authentication** strongly correlate with fraud.
- Higher **shipping distance** is associated with increased fraud risk.
- Fraud distribution varies across **transaction channels** and **merchant categories**.

---

## 🧠 Modeling Approach
The problem is framed as a **binary classification task**.

### Models Implemented:
- Logistic Regression (baseline)
- Random Forest Classifier
- Gradient Boosting Classifier

### Evaluation Metrics:
Due to class imbalance, the following metrics were prioritized:
- Precision
- Recall
- F1-score
- Confusion Matrix

Accuracy was not used as the primary metric due to its limitations in fraud detection scenarios.

---

## 🚀 How to Run the Project
1. Clone the repository:
```bash
git clone <repository-url>
cd ecommerce-fraud-detection
```
---
## 🧠 Learnings

Importance of proper EDA before modeling

Handling class imbalance using SMOTE

Building modular and reusable ML pipelines

Model persistence using joblib

Accuracy alone is not sufficient for churn problems

---

## 📌 Future Improvements

Hyperparameter tuning (GridSearchCV)

Model deployment using Streamlit or Flask

Recall-focused optimization

Real-time prediction interface

---

## 👤 Author

**Shivam Singh**
Aspiring Data Scientist | Machine Learning Enthusiast

🔗 GitHub: [https://github.com/shivamsingh-itds]
🔗 LinkedIn: [www.linkedin.com/in/shivamsinghds]

---

⭐ If you find this project helpful, feel free to star the repository!
