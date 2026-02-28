# Fraud Detection in Financial Transactions using Machine Learning

## 📌 Project Overview
This project focuses on detecting fraudulent financial transactions using Machine Learning techniques. 
The model is trained on a highly imbalanced dataset where fraudulent transactions are very rare (~0.13%).

The goal is to accurately identify fraudulent transactions while minimizing false negatives.

---

## 🚀 Features
- Data cleaning and preprocessing
- Handling imbalanced dataset
- Feature engineering (balance differences)
- XGBoost classification model
- Threshold tuning for better fraud detection
- Model evaluation using multiple metrics

---

## 📊 Dataset
- Large dataset with over 6 million transactions
- Highly imbalanced (~0.13% fraud cases)
- Includes transaction details such as:
  - Transaction type
  - Amount
  - Account balances

---

## 🧠 Approach

### 1. Data Cleaning
- Removed missing values
- Dropped irrelevant columns (nameOrig, nameDest)
- Analyzed outliers using IQR method

### 2. Feature Engineering
- Created new features like balance differences

### 3. Handling Imbalance
- Used `scale_pos_weight` in XGBoost
- Focused on improving recall

### 4. Model
- XGBoost Classifier
- Hyperparameter tuning using RandomizedSearchCV

### 5. Threshold Tuning
- Adjusted decision threshold to improve fraud detection
- Selected optimal threshold (~0.01)

---

## 📈 Model Performance
- ROC-AUC Score: ~0.99
- High Recall (~88% - 96%) for fraud detection
- Balanced precision and recall using threshold tuning

---

## 🔍 Key Insights
- Fraud is more common in TRANSFER and CASH_OUT transactions
- High transaction amounts are often suspicious
- Sudden balance changes indicate potential fraud

---

## 🛠️ Technologies Used
- Python
- Pandas, NumPy
- Scikit-learn
- XGBoost
- Matplotlib

---

## 📌 Conclusion
The model performs well in detecting fraudulent transactions with high recall and ROC-AUC score. 
Threshold tuning and imbalance handling significantly improved the model's performance.

---

## 📎 Future Improvements
- Deploy model using Streamlit
- Real-time fraud detection system
- Use deep learning models

---

## 👨‍💻 Author
Utkarsh Srivastav
