# Customer Churn Prediction

## 📌 Project Overview
Customer churn is a critical problem for subscription-based businesses. This project aims to predict whether a customer is likely to churn based on demographic details, service usage, and billing behavior, enabling businesses to take proactive retention measures.

---

## 📊 Dataset
- Telecom Customer Churn Dataset
- Approximately 7,000 customer records
- Features include:
  - Demographics (gender, senior citizen)
  - Account information (tenure, contract type)
  - Services subscribed (internet, tech support)
  - Billing and payment methods

---

## ⚙️ Tech Stack
- Python  
- Pandas, NumPy  
- Matplotlib, Seaborn  
- Scikit-learn  
- Imbalanced-learn (SMOTE)  
- Jupyter Notebook  

---

## 🧪 Project Workflow

### 1. Data Cleaning & Preprocessing
- Handled missing values
- Encoded categorical variables
- Scaled numerical features

### 2. Exploratory Data Analysis (EDA)
- Identified high churn among:
  - Month-to-month contract customers
  - Electronic check payment users
  - Customers without tech support
- Visualized trends using bar plots, box plots, histograms, and heatmaps

### 3. Handling Class Imbalance
- Applied **SMOTE** to balance churn vs non-churn classes
- Compared model performance **before and after SMOTE**

### 4. Model Building
- Logistic Regression
- Random Forest
- Gradient Boosting

### 5. Model Evaluation
- Accuracy, Precision, Recall, F1-score
- ROC-AUC Curve
- Confusion Matrix

### 6. Model Selection & Saving
- Selected the best-performing model based on recall and ROC-AUC
- Saved the trained model using `joblib` for future deployment

---

## 📈 Key Insights
- Customers on month-to-month contracts are significantly more likely to churn
- Lack of technical support strongly correlates with higher churn
- Applying SMOTE improved recall for churned customers, reducing false negatives

---

## 🚀 Future Improvements
- Deploy the model using Flask or FastAPI
- Add real-time prediction support
- Experiment with cost-sensitive learning techniques
