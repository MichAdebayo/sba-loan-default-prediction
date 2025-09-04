# Small Business Loan Default Prediction

<p align="center">
   <img width=800 alt="SBA Loan Prediction" src="https://github.com/user-attachments/assets/90fa72c2-1844-4e59-8a61-ee498ddfe237" />
</p>

## Project Overview
This project is focused on predicting whether a small business in the United States will default on an SBA (Small Business Administration) loan. Given the critical role of small businesses in job creation and economic growth, accurate loan default prediction can help financial institutions make informed lending decisions, mitigate risks, and support business sustainability.

## Context
As a Data Scientist at the **United States Small Business Administration (US SBA)**, your role is to develop a machine learning model to assess the risk of loan default before granting loans. The challenge is to perform binary classification (i.e., **should the loan be granted? Yes or No**). 

## Data Considerations & Challenges

### **Data Leakage**
One of the most important aspects of this project is to **avoid data leakage**. This means that features that would not be available at the time of loan approval should not be used for prediction. For example:
- The **total amount repaid** should not be used, as it is only available after the loan has been granted.
- Features derived from future events should be carefully considered to prevent biased results.

### **Performance Metrics**
Since this is a classification problem, we need to evaluate the model using appropriate metrics such as:
- **Confusion Matrix**
- **ROC-AUC Score**
- **Precision & Recall**
- **F1 Score**

A well-balanced approach to these metrics is critical to ensure that the model minimizes false negatives (approving bad loans) while maintaining a reasonable false positive rate (rejecting good loans).

---

## Project Workflow
This project is divided into two major phases:

### **Phase 1: Data Cleaning, Exploration & Feature Engineering (EDA)**
- Load and inspect the dataset.
- Handle missing values and outliers.
- Perform **univariate** and **bivariate** analysis.
- Conduct statistical tests where necessary.
- Engineer new features and perform feature selection.

### **Phase 2: Model Training & Evaluation**
- Prepare the dataset for modeling (train-test split, scaling, encoding, etc.).
- Implement and evaluate multiple models:
  - **Logistic Regression**
  - **Boosting models**: **XGBoost**, **CatBoost**, **LightGBM**
- Interpret model outputs:
  - Feature importance analysis.
  - **Bonus**: Use SHAP values for explainability.

---

## Implementation
The project is implemented using **Jupyter Notebooks**, where the following steps are documented:
1. **Data Cleaning & Preprocessing:** Handling missing values, outliers, encoding categorical variables, and feature selection.
2. **Exploratory Data Analysis (EDA):** Visualizing distributions, correlations, and key insights.
3. **Modeling & Evaluation:** Training various models, hyperparameter tuning, and assessing model performance.
4. **Feature Importance & Explainability:** Understanding which features influence loan repayment predictions.

---

## Tools & Libraries Used
- **Python**
- **Pandas, NumPy** (Data manipulation & analysis)
- **Matplotlib, Seaborn** (Data visualization)
- **Scikit-learn** (Machine learning models & metrics)
- **XGBoost, CatBoost, LightGBM** (Boosting algorithms)
- **SHAP** (Feature interpretability)
- **Jupyter Notebook** (Code execution & documentation)

---

## Usage

### **Running the Notebooks**
1. Clone the repository:
   ```bash
   git clone <https://github.com/MichAdebayo/brief-loan-prediction>
   cd brief-loan-prediction
   ```
2. Install required dependencies:
   ```bash
   pip install -r requirements.txt
   ```
3. Open Jupyter Notebook and run the analysis:
   ```bash
   jupyter notebook
   ```

---

## Conclusion
This project provides an end-to-end solution for predicting small business loan defaults using machine learning. The insights and models developed can help financial institutions and policymakers make data-driven lending decisions while minimizing risks. Future work can include:
- Implementing additional models and ensemble techniques.
- Deploying the model as an API for real-time loan approval predictions.
- Incorporating alternative data sources for enhanced predictive performance.

For further improvements or contributions, feel free to open an issue or submit a pull request!

---

## Author
- [Michael ADEBAYO](https://github.com/MichAdebayo/)
- [Maxime FLAVIGNY](https://github.com/TheMaxfly)