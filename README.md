# `Telecom-Customer-Churn-Prediction`
An end-to-end machine learning project focused on predicting telecom customer churn and analyzing the factors associated with customer attrition.

### `Introduction`
- The dataset contains information about 7,043 telecom customers.
- It includes 21 original features related to customer demographics, services, contracts, and billing.
- The target variable is Churn, which indicates whether a customer left the company.
- Customer information includes gender, senior citizen status, partner, and dependents.
- Service-related features include Internet Service, Online Security, Tech Support, Streaming Services, and more.
- Contract and billing information includes tenure, contract type, payment method, monthly charges, and total charges.
- The dataset is used to analyze customer behavior and build a machine learning model to predict churn.

### `Problem Statement`
- Telecom companies face customer churn, where customers discontinue their services.
- High customer churn can lead to revenue loss and increased customer acquisition costs.
- It can be difficult to identify which customers are more likely to churn.
- Different factors such as contract type, tenure, services, payment method, and monthly charges may influence churn.

### `Dataset Used`
<a href="https://github.com/alinasingh/Telecom-Customer-Churn-Prediction/blob/main/WA_Fn-UseC_-Telco-Customer-Churn.csv">Customer Prediction Dataset

### `Project Objectives`
- Analyze customer data to understand patterns and factors associated with churn.
- Perform data cleaning and exploratory data analysis (EDA) to prepare the dataset.
- Apply feature engineering to create meaningful features for the machine learning model.
- Build and compare machine learning models for customer churn prediction.
- Evaluate model performance using metrics such as Accuracy, Precision, Recall, F1-Score, ROC-AUC, and Confusion Matrix.
- Identify the key factors influencing customer churn.
- Tune the prediction threshold to achieve a better balance between precision and recall for churned customers.

### `Technologies Used`
- Python
- Pandas — Data manipulation and analysis
- NumPy — Numerical operations
- Matplotlib & Seaborn — Data visualization
- Scikit-learn — Data preprocessing, model building, and evaluation
- Jupyter Notebook — Development environment

### `Exploratory Data Analysis`
- Analyzed the distribution of the target variable `Churn`.
- Examined customer demographics such as gender, senior citizen status, partner, and dependents.
- Analyzed the relationship between customer services and churn.
- Studied the impact of contract type and payment method on customer churn.
- Analyzed the relationship between tenure, monthly charges, and churn.
- Identified patterns and customer segments with higher churn rates.
- Used visualizations to understand key factors associated with customer attrition.

### `Feature Engineering`
- Created meaningful features to better represent customer behavior.
- Grouped customers based on their **tenure** to identify different customer lifecycle stages.
- Created customer service-related features to understand the relationship between the number of services and churn.
- Calculated **Average Monthly Spend** to capture customer spending behavior.
- Analyzed engineered features to determine their relationship with customer churn.
- Selected relevant features for the machine learning models.

### `Machine Learning Models`
- Split the dataset into **training and testing sets**.
- Applied preprocessing techniques to prepare numerical and categorical features.
- Trained a **Logistic Regression** model as the baseline model.
- Trained a **Random Forest Classifier** for comparison.
- Evaluated both models using **Accuracy, Precision, Recall, F1-Score, ROC-AUC, and Confusion Matrix**.
- Performed **classification threshold tuning** to improve the detection of churned customers.
- Compared model performance and selected the approach based on the project's churn-prediction objective.

### `Model Performance & Results`

### Logistic Regression
- Accuracy: **80.17%**
- ROC-AUC: **0.8364**
- Churn Recall: **55%**
- Churn F1-Score: **59%**

### Random Forest
- Accuracy: **78.75%**
- ROC-AUC: **0.8189**
- Churn Recall: **50%**
- Churn F1-Score: **55%**

### Threshold-Tuned Model
After tuning the classification threshold to improve churn detection:
- Accuracy: **79%**
- Churn Precision: **59%**
- Churn Recall: **68%**
- Churn F1-Score: **63%**

The threshold-tuned model improved the detection of customers likely to churn, increasing churn recall from **55% to 68%** while maintaining a reasonable balance between precision and recall.

### `Key Business Insights`
- Customers on **month-to-month contracts** have a significantly higher churn rate compared with customers on longer-term contracts.
- Customers using **electronic check** as their payment method show a higher likelihood of churn.
- Customers without services such as **Online Security** and **Tech Support** tend to have higher churn rates.
- **Newer customers** are more likely to churn compared with customers who have stayed with the company for a longer period.
- Higher customer churn is associated with certain combinations of **contract type, services, payment methods, and customer tenure**.
- These insights can help telecom companies identify high-risk customers and develop targeted **retention strategies**.


## `Conclusion`

This project developed an end-to-end machine learning solution for predicting customer churn in the telecom industry. Through data cleaning, exploratory data analysis, feature engineering, and machine learning, the project identified important factors associated with customer attrition.

Logistic Regression and Random Forest were evaluated, with Logistic Regression achieving the better baseline ROC-AUC score. Classification threshold tuning further improved the model's ability to identify customers likely to churn, increasing churn recall to **68%** and the churn F1-score to **63%**.

The analysis provides useful insights that can help telecom companies identify high-risk customers and develop targeted customer retention strategies.

