# customer_churn_pred

# Telecom Customer Churn Prediction

## 📌 Project Overview

This project focuses on predicting **customer churn** (whether a customer will leave or stay) in a telecom company. Churn prediction is important for businesses because retaining existing customers is often cheaper than acquiring new ones.

The dataset includes customer information such as demographics, account details, and services subscribed. Using this data, we apply **machine learning models** to predict churn.

---

## 📂 Dataset

- **Source**: Telco Customer Churn dataset (commonly used for churn prediction tasks).
- **Features**:
  - Demographics (e.g., gender, senior citizen, partner, dependents).
  - Services (e.g., phone, internet, online security, streaming).
  - Account information (e.g., contract type, payment method, monthly charges, tenure).
- **Target**: `Churn` (Yes/No).

---

## ⚙️ Preprocessing

- Handled missing values.
- Encoded categorical features using:
  - **Manual mapping** (e.g., contract type).
  - **Label Encoding** (e.g., gender, churn).
  - **One-Hot Encoding** (e.g., payment method, internet service).
- Scaled numerical features.
- Balanced the dataset using **SMOTE** to handle class imbalance.

---

## 🤖 Models Used

- Logistic Regression
- Decision Tree
- Random Forest
- Gradient Boosting
  ... I'm learning I tried a lot of things

Hyperparameter tuning was performed using **GridSearchCV**.

---

## 📊 Results

- Best model: **Random Forest** (after hyperparameter tuning).
- Evaluation metrics: Accuracy, Precision, Recall, F1-score, ROC-AUC.
- The model helps identify customers at risk of leaving, so retention strategies can be applied.

---

## 💾 Model Saving

- **Best Model** → saved as `best_model.pkl`.
- **Encoders** → saved as `encoders.pkl`.
- **Scaler** → saved as `scaler.pkl`.

This allows reusing the model for predictions on new customer data.

---

## 📌 Future Improvements

Try deep learning models (e.g., Neural Networks).
Deploy the model with a Flask/Django API.
Create a dashboard for visualization (Streamlit/Power BI/Tableau).
