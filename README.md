🏦 Loan Default Prediction Using Decision Tree
This project predicts whether a loan application will be approved or not based on applicant details using machine learning (Decision Tree Classifier).

📁 Dataset
Name: Loan Prediction Dataset

File: train_u6lujuX_CVtuZ9i.csv

Source: Provided in ZIP format (uploaded manually)

Features include:

Gender

Marital Status

Education

Applicant Income

Credit History

Loan Amount

And more...

Target Column:

Loan_Status (1 = Loan Approved, 0 = Not Approved)

🔧 Technologies Used
Python 🐍

Google Colab for execution

Libraries:

pandas, numpy – data handling

matplotlib, seaborn – data visualization

sklearn – model training and evaluation

zipfile, os, google.colab – file handling in Colab

⚙ Preprocessing Steps
Dropped Loan_ID as it's just an identifier

Handled missing values:

Categorical columns: filled with mode

Numerical columns: filled with median

Encoded categorical features using LabelEncoder

🧠 Model Training
Trained two models:

✅ Decision Tree Classifier (main model)

✅ (Optional) Random Forest Classifier for comparison

🔢 Code Snippet:
python
Copy
Edit
model = DecisionTreeClassifier(random_state=42)
model.fit(X_train, y_train)
y_pred = model.predict(X_val)
print("Accuracy:", accuracy_score(y_val, y_pred))
print(classification_report(y_val, y_pred))
📈 Output (Decision Tree Results)
markdown
Copy
Edit
Accuracy: 0.75

              precision    recall  f1-score   support

           0       0.71      0.68      0.70        25
           1       0.77      0.79      0.78        35

    accuracy                           0.75        60
   macro avg       0.74      0.74      0.74        60
weighted avg       0.75      0.75      0.75        60
✅ Conclusion:
The Decision Tree model achieved an accuracy of 75%, with a balanced precision and recall. Feature importance analysis showed which applicant features had the most influence on loan approval decisions.
