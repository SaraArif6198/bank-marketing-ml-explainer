# Task01- Bank Marketing Term Deposit Prediction

##  Task Objective

The objective of this project is to predict whether a bank customer will subscribe to a term deposit as a result of a direct marketing campaign, using the **Bank Marketing Dataset** from the UCI Machine Learning Repository. The project also includes interpreting model predictions using Explainable AI (XAI) techniques such as **SHAP** and **LIME**.

##  Approach

### 1. Data Exploration & Preprocessing
- Loaded and explored the dataset for structure and key patterns.
- Encoded all categorical variables using one-hot encoding.
- Handled missing or unknown values appropriately.

### 2. Modeling
- Trained two classifiers:
  - **Logistic Regression**
  - **Random Forest**
- Evaluated both models using:
  - **Confusion Matrix**
  - **F1-Score**
  - **ROC Curve**

### 3. Explainability
- Applied **SHAP** to explain global and local feature contributions for Logistic Regression.
- Applied **LIME** to explain individual prediction logic.
- Compared SHAP and LIME visually and interpretively.


## ✅ Results and Findings

###  Key Features Influencing Subscription:
- `duration` (call length) is the most influential positive feature.
- `contact_unknown`, `housing_yes`, `loan_yes`, and `poutcome_success` contributed negatively in most predictions.

###  Model Evaluation:
- Both Logistic Regression and Random Forest performed well, with competitive F1-scores and ROC curves.

###  Explainability Insights:
- **SHAP** provided both global and individual feature importance plots.
- **LIME** offered interpretable decision rules for single instances.
- Consistency between SHAP and LIME enhances trust in model predictions.

###  Business Recommendations:
- Focus on customers with longer engagement (call duration).
- Target past successful clients for better campaign efficiency.
- Avoid unreliable contact methods like "unknown".
- Optimize campaign months (e.g., prioritize August, avoid March).

## 📦 Packages Used

| Package             | Purpose                                         |
|---------------------|-------------------------------------------------|
| `pandas`            | Data manipulation and cleaning                  |
| `numpy`             | Numerical operations                            |
| `matplotlib`        | Data visualization                              |
| `seaborn`           | Enhanced statistical plots                      |
| `scikit-learn`      | Modeling, preprocessing, and evaluation         |
| `shap`              | SHAP explainability for global/local insights   |
| `lime`              | LIME for local explanation of individual predictions |
| `IPython`           | (Optional) For interactive display in notebooks |


## 📂 Files Included

- `notebook.ipynb`: Complete Jupyter Notebook
- `requirements.txt`: List of required packages
- `README.md`: Project overview

## 🔗 Dataset

- UCI Repository: [Bank Marketing Dataset](https://archive.ics.uci.edu/ml/datasets/bank+marketing)

---
📨 Submitted as part of the DeveloperHub Internship Program
