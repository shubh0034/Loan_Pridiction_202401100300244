# 🏦 Loan Default Prediction Using Decision Tree

This project predicts whether a loan application will be approved or not based on applicant details using machine learning (Decision Tree Classifier).

## 📁 Dataset

- *Name*: Loan Prediction Dataset  
- *File*: train_u6lujuX_CVtuZ9i.csv  
- *Source*: Provided in ZIP format (uploaded manually)

The dataset contains features like:
- Gender
- Marital Status
- Education
- Applicant Income
- Credit History
- Loan Amount
- And more...

Target Column:
- Loan_Status (1 = Loan Approved, 0 = Not Approved)

---

## 🔧 Technologies Used

- Python 🐍
- Google Colab (for running the notebook)
- Libraries:
  - pandas, numpy – data handling
  - matplotlib, seaborn – data visualization
  - sklearn – model training and evaluation
  - zipfile, os, google.colab – file extraction and handling in Colab

---

## ⚙ Preprocessing Steps

- Dropped Loan_ID as it's just an identifier
- Filled missing values:
  - *Categorical columns* with Mode
  - *Numerical columns* with Median
- Encoded categorical variables using LabelEncoder

---

## 🧠 Model Training

Used two models:
- ✅ *Decision Tree Classifier* (main)
- ✅ (Optional) *Random Forest Classifier* for better accuracy

### Code Snippet:
```python
model = DecisionTreeClassifier(random_state=42)
model.fit(X_train, y_train)# Loan_Pridiction_202401100300244
