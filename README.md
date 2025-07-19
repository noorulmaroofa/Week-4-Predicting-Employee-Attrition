# Predicting Employee Attrition with IBM HR Analytics Dataset

## Objective

This project aims to predict whether an employee is likely to leave the company using IBM’s HR analytics data. By leveraging machine learning techniques and data analysis, the goal is to help HR departments take proactive measures to retain valuable employees.

---

## Dataset

**Source**: [Kaggle - IBM HR Analytics Employee Attrition Dataset](https://www.kaggle.com/datasets/pavansubhasht/ibm-hr-analytics-attrition-dataset)

The dataset includes employee attributes like:

- Age, Gender, Monthly Income
- Job Role, Department, Job Satisfaction
- Overtime, Work Life Balance, Environment Satisfaction
- Attrition status (target variable)

---

## Tools & Libraries Used

- **Language**: Python
- **Platform**: Google Colab / Jupyter Notebook
- **Libraries**:
  - `pandas`, `numpy` – Data handling
  - `matplotlib`, `seaborn` – Visualization
  - `scikit-learn` – ML algorithms and metrics
  - `imbalanced-learn` – SMOTE for handling class imbalance
  - `xgboost` – Advanced tree-based modeling
  - `shap` – Model explainability

---

## Project Workflow

### 1. Load and Explore the Data

- Understand data structure using `.info()`, `.describe()`, and value counts
- Visualize class distribution and categorical features

### 2. Data Preprocessing

- Label encode binary columns
- One-hot encode categorical variables
- Scale numerical features
- Drop irrelevant columns
- Handle class imbalance using **SMOTE**

### 3. Exploratory Data Analysis (EDA)

- Count plots for categorical variables
- Box plots for numerical comparisons
- Correlation heatmap

### 4. Model Building

- Logistic Regression
- Random Forest Classifier
- XGBoost Classifier

### 5. Model Evaluation

- Accuracy, Precision, Recall, F1-score
- Confusion Matrix
- Focus on **Recall** to catch likely resignations

### 6. Feature Importance

- Feature importance from Random Forest
- SHAP values for model explainability

---

## Results & Insights

- **XGBoost** and **Random Forest** provided strong performance.
- Important predictors of attrition:
  - `OverTime`, `JobSatisfaction`, `EnvironmentSatisfaction`, `MonthlyIncome`
- SHAP visualizations showed clear feature contributions to attrition risk.

---

## Conclusion

This model helps HR teams:

- Identify at-risk employees
- Take preventive actions (e.g., job rotation, salary hikes, flexible hours)
- Reduce attrition rates and retain top talent

## File Structure

├── Employee*Attrition_Prediction.ipynb
├── README.md
├── WA_Fn-UseC*-HR-Employee-Attrition.csv

---

## Author

**Noorul Maroofa**  
[LinkedIn Profile](https://www.linkedin.com/in/noorul-maroofa-145b17343/)

---

## Note

This project was completed as part of a data science internship assignment.  
All visuals, code, and results are intended for educational and analytical purposes.
