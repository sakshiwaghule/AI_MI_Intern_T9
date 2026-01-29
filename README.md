# AI_MI_Intern_T9
# Credit Card Fraud Detection 
#Overview
This dataset contains transactions made by credit cards in September 2013 by European cardholders. It is a subset containing **999 transactions**, used primarily for practicing fraud detection and handling extreme class imbalance.
#Data Structure
* **Total Records:** 999
* **Total Features:** 30 (plus the target class)
* **Columns:**
* `Time`: Seconds elapsed between each transaction and the first transaction in the dataset.
* `V1 - V28`: Principal components obtained with PCA (anonymized features to protect user identity).
* `Amount`: The transaction amount.
* `Class`: The target variable (**1** for Fraud, **0** for Non-fraud).
#Class Distribution
The dataset is highly imbalanced, which is typical for fraud detection tasks:
* **Non-fraud (Class 0):** 997 transactions (99.8%)
* **Fraud (Class 1):** 2 transactions (0.2%)
#Key Insights from Analysis
* **Top Fraud Indicators:** Feature importance analysis via Random Forest suggests that variables **V10, V11, and V4** are the most significant predictors in identifying fraudulent activity.
* **Model Performance:** While baseline models (Logistic Regression) and Random Forest achieved **100% accuracy**, this is primarily due to the majority class (non-fraud). For this dataset, metrics like **Precision, Recall, and F1-Score** are critical for evaluating true performance.
