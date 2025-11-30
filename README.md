# 🔮 Customer Churn Prediction – Machine Learning Project

A complete end-to-end Machine Learning project using the **Telco Customer Churn dataset**.  
This project predicts whether a customer is likely to churn based on service usage, contract type, tenure, payment methods, and demographic features.

The goal is to build a clean, beginner-friendly classification model while showcasing essential Data Science skills:
✔ Data cleaning  
✔ Exploratory Data Analysis (EDA)  
✔ Feature encoding  
✔ Train/Test split  
✔ Logistic Regression & Random Forest  
✔ Model evaluation & visualization  
✔ Saving deployable ML model  
✔ Extracting business insights  

---

## 📂 Dataset  
**Source:** Telco Customer Churn (Kaggle)

**Rows:** 7043  
**Columns:** 21  

Key fields include:  
- `gender`, `SeniorCitizen`, `Partner`, `Dependents`  
- `tenure`, `InternetService`, `Contract`  
- `PaymentMethod`, `MonthlyCharges`, `TotalCharges`  
- `Churn` (target column)

---

## 🛠️ Technologies Used
- Python  
- Pandas  
- NumPy  
- Matplotlib  
- Seaborn  
- Scikit-learn  
- Joblib  

---

## 📊 Project Steps

### **1. Data Cleaning**
- Converted `TotalCharges` from object → float  
- Filled missing values with median  
- Removed `customerID`  
- Encoded categorical variables using Label Encoding  

### **2. Exploratory Analysis**
- Tenure trends  
- Monthly charges distribution  
- Contract type effect on churn  
- Correlation heatmap  

### **3. Machine Learning Models**
#### **Logistic Regression**
- Baseline model  
- Accuracy: ~0.79  

#### **Random Forest Classifier**
- Tuned hyperparameters  
- Accuracy achieved: **0.80+**  
- Feature importance used to understand key drivers of churn  

### **4. Visualizations**
- Confusion Matrix  
- Top 15 Feature Importances  
- Distribution plots  

### **5. Model Export**
The final model is saved as:

```
churn_model.pkl
```

---

## 📈 Key Insights (full version in insights.txt)

- Customers on **month-to-month contracts** churn the most  
- **Long-term tenure** strongly reduces churn  
- **Electronic Check** users churn at the highest rate  
- **Fiber Optic** users churn more than DSL customers  
- Customers with **high monthly charges** have higher churn probability  

---

## 📁 Repository Structure

```
Customer-Churn-Prediction/
├── churn_notebook.ipynb
├── telco_churn.csv
├── churn_model.pkl
├── insights.txt
├── README.md
└── figures/
     ├── confusion_matrix.png
     └── feature_importance.png
```

---

## 🚀 How to Run  
1. Clone the repository  
2. Install requirements  
3. Open and run `churn_notebook.ipynb`  
4. To load the trained model:

```python
import joblib
model = joblib.load("churn_model.pkl")
```

---

## 👨‍💻 Author  
**Vivek S. Chindalia**  
B.E. Information Technology – Mumbai University  
📧 chindaliavivek@gmail.com












