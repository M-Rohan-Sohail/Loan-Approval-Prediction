# 💰 Loan Approval Prediction using Random Forest Classifier

This project predicts **loan approval status** (Approved/Rejected) using a machine learning model built with a **Random Forest Classifier**.  
It helps understand how different factors like income, loan amount, CIBIL score, and employment status affect loan decisions.

---

## 🚀 Project Overview
The dataset contains details about applicants such as education, employment status, annual income, loan amount, loan term, and CIBIL score.  
The objective is to classify whether a loan should be **approved** or **rejected**.

---

## 🧩 Data Preprocessing
Categorical features were label-encoded for model compatibility:
- `education` → Graduate: 1, Not Graduate: 0  
- `self_employed` → Yes: 1, No: 0  
- `loan_status` → Approved: 1, Rejected: 0  

---

## ⚙️ Model Details
- **Algorithm Used:** Random Forest Classifier  
- **Train-Test Split:** 70/30  
- **Hyperparameters:**  
  - `n_estimators = 500`  
  - `max_depth = 9`  
  - `class_weight = 'balanced'` (to handle class imbalance)

---

## 📊 Evaluation Metrics
The model was evaluated using key classification metrics:

| Metric | Train | Test |
|:--------|:-------------:|:------------:|
| **Accuracy** | 0.9997 | 0.9758 |

### 🔢 Confusion Matrix (Test)
[[460 11]
[ 20 790]]

### 📋 Classification Report (Test)
| Class | Precision | Recall | F1-Score | Support |
|:------|:-----------:|:--------:|:----------:|:----------:|
| 0 (Rejected) | 0.96 | 0.98 | 0.97 | 471 |
| 1 (Approved) | 0.99 | 0.98 | 0.98 | 810 |

**Macro Avg:** Precision = 0.97 | Recall = 0.98 | F1 = 0.97  
**Weighted Avg:** Precision = 0.98 | Recall = 0.98 | F1 = 0.98  

---

## ✅ Conclusion
The model achieved **97.6% accuracy** on the test data with excellent recall and precision balance.  
Using `class_weight='balanced'` helped handle potential class imbalance effectively.  
The model generalizes well and is robust without overfitting.

---

## 🛠️ Tech Stack
- **Language:** Python  
- **Libraries:** Pandas, Scikit-learn 

---

## 📚 Future Work
- Perform hyperparameter tuning using GridSearchCV or RandomizedSearchCV  
- Experiment with XGBoost and LightGBM  
- Add feature importance visualization and SHAP interpretability

---

## ✨ Author
**Muhammad Rohan Sohail**  
🎓 BSc Electrical Engineering @ UET Lahore  
💡 Machine Learning & Data Science Enthusiast  
