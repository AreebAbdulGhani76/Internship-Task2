# Internship-Task2
# Task 1: Term Deposit Subscription Prediction (Bank Marketing)

# Task Objective

The objective of this project is to predict whether a bank customer will subscribe to a term deposit based on the results of a marketing campaign. The dataset used for this task is the Bank Marketing Dataset from the UCI Machine Learning Repository.
The goal is to build classification models that can analyze customer behavior and help banks improve their marketing strategies.

# Dataset

The dataset contains information about bank clients such as:

Age
Job
Marital status
Education
Account balance
Contact type
Duration of call
Campaign information

Target variable:
y → whether the client subscribed to a term deposit (yes/no)

# Approach
1. Data Exploration

The dataset was loaded and explored using pandas to understand the structure, features, and distribution of the data.

2. Data Preprocessing

Categorical variables were encoded using appropriate encoding techniques to convert them into numerical form suitable for machine learning models.

3. Model Training

Two classification models were trained:

Logistic Regression
Random Forest Classifier

These models were used to predict whether a customer will subscribe to a term deposit.

4. Model Evaluation

The models were evaluated using the following metrics:

Confusion Matrix
F1 Score
ROC Curve

These metrics help measure classification performance and model reliability.

5. Model Interpretability

To understand the decision-making process of the models, Explainable AI techniques were used.

SHAP (SHapley Additive Explanations)
or
LIME (Local Interpretable Model-Agnostic Explanations)

These techniques were used to explain at least 5 individual predictions, highlighting which features influenced the model's decisions.

# Results and Findings

The models successfully predicted customer subscription behavior.
Random Forest generally performed better due to its ability to capture complex relationships in the data.
Features such as call duration, campaign contacts, and customer profile information were important predictors.
SHAP/LIME explanations helped interpret how individual features influenced model predictions.
