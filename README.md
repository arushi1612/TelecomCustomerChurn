# Telecom Customer Churn Prediction
<p align='center'>
<img src ='https://github.com/user-attachments/assets/9eaf652d-e1d4-4031-b1ca-2f5228cc5b10'/>
</p>

## Project Overview
Telecom customer churn prediction involves identifying which customers are likely to cancel their subscription to a telecom service based on their usage patterns and behaviors. This is particularly crucial in the telecom industry, where retaining customers is essential for maintaining a stable and profitable business.
## Why is it important?
Customer churn is a prevalent issue across various sectors, including the telecom industry. To grow as a telecom company, substantial investment is required to acquire new clients. When a customer leaves, it represents a significant loss of investment. The time and effort spent on acquiring and servicing that customer need to be redirected towards replacing them. By predicting when a telecom customer is likely to leave and offering them incentives to stay, a company can achieve considerable savings. This proactive approach not only retains customers but also enhances overall business efficiency and profitability.
## Dataset
The dataset used for this analysis is from a telecom company and can be found here. It contains various customer attributes such as demographics, account information, and services subscribed. The dataset has 7043 entries and 20 features.

**Features:**
* **gender:** Gender of the customer (Female, Male)
* **SeniorCitizen:** Indicates if the customer is a senior citizen (0: No, 1: Yes)
* **Partner:** Indicates if the customer has a partner (Yes, No)
* **Dependents:** Indicates if the customer has dependents (Yes, No)
* **tenure:** Number of months the customer has stayed with the company
* **PhoneService:** Indicates if the customer has phone service (Yes, No)
* **MultipleLines:** Indicates if the customer has multiple lines (No phone service, No, Yes)
* **InternetService:** Type of internet service (DSL, Fiber optic, No)
* **OnlineSecurity:** Indicates if the customer has online security (No, Yes, No internet service)
* **OnlineBackup:** Indicates if the customer has online backup (Yes, No, No internet service)
* **DeviceProtection:** Indicates if the customer has device protection (No, Yes, No internet service)
* **TechSupport:** Indicates if the customer has tech support (No, Yes, No internet service)
* **StreamingTV:** Indicates if the customer has streaming TV (No, Yes, No internet service)
* **StreamingMovies:** Indicates if the customer has streaming movies (No, Yes, No internet service)
* **Contract:** Contract term of the customer (Month-to-month, One year, Two year)
* **PaperlessBilling:** Indicates if the customer uses paperless billing (Yes, No)
* **PaymentMethod:** Payment method (Electronic check, Mailed check, Bank transfer (automatic), Credit card (automatic))
* **MonthlyCharges:** The amount charged to the customer monthly
* **TotalCharges:** The total amount charged to the customer
* **Churn:** Indicates if the customer churned (Yes, No)

## Key Steps
### Data Preprocessing:
- *Null and Missing Values:* Detected and appropriately handled null and missing values.
- *Duplicate Values:* Identified and removed any duplicated entries.

### Exploratory Data Analysis (EDA):
- *Univariate Analysis:* Conducted univariate analysis on numerical and categorical features to understand their distribution.
- *Bivariate Analysis:* Performed bivariate analysis to explore the relationship and trends between features and the target variable (Churn). Identified any outliers present.

### Encoding Variables:
- *Independent Variables:* Applied one-hot encoding and ordinal encoding to transform categorical independent variables.
- *Target Variable:* Utilized label encoding for the target variable, Churn.

### Feature Selection:
- Employed statistical tests such as the Z-test and Chi-square test to analyze the association between numerical/categorical variables and Churn. Dropped variables based on their significance.

### Model Training and Evaluation:
- *Model:* Trained a logistic regression model to predict customer churn.
- *Evaluation Metrics:* Evaluated the model using recall and ROC curve.

### Handling Imbalanced Data:
- *Class Weights:* Managed class imbalance in the churn data by adjusting class weights.

### Assumption Validation:
- *Multicollinearity:* Checked for multicollinearity using the Variance Inflation Factor (VIF).
- *Linearity:* Assessed linearity assumptions.
- *Residual Analysis:* Conducted residual analysis and made necessary adjustments.

### Hyperparameter Tuning:
- *Techniques:* Used Grid Search CV and RandomizedSearchCV for parameter optimization.

