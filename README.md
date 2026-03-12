# Data Science & Analytics Interns Task2
# Task1: Term Deposit Subscription Prediction (Bank Marketing)

# 📌Objective:

The objective of this project is to predict whether a bank customer will subscribe to a term deposit based on the results of a marketing campaign. The dataset used for this task is the Bank Marketing Dataset from the UCI Machine Learning Repository.
The goal is to build classification models that can analyze customer behavior and help banks improve their marketing strategies.

# 📊Dataset

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

# 🛠️Approach:

# 1️⃣ Data Exploration

The dataset was loaded and explored using pandas to understand the structure, features, and distribution of the data.

# 2️⃣ Data Preprocessing

Categorical variables were encoded using appropriate encoding techniques to convert them into numerical form suitable for machine learning models.

# 3️⃣ Model Training

Two classification models were trained:

Logistic Regression
Random Forest Classifier

These models were used to predict whether a customer will subscribe to a term deposit.

# 4️⃣ Model Evaluation

The models were evaluated using the following metrics:

Confusion Matrix
F1 Score
ROC Curve

These metrics help measure classification performance and model reliability.

# 5️⃣Model Interpretability

To understand the decision-making process of the models, Explainable AI techniques were used.

SHAP (SHapley Additive Explanations)
or
LIME (Local Interpretable Model-Agnostic Explanations)

These techniques were used to explain at least 5 individual predictions, highlighting which features influenced the model's decisions.

# 📈Results and Findings:

1) The models successfully predicted customer subscription behavior.
2) Random Forest generally performed better due to its ability to capture complex relationships in the data.
3) Features such as call duration, campaign contacts, and customer profile information were important predictors.
4) SHAP/LIME explanations helped interpret how individual features influenced model predictions.

## Task 2: Customer Segmentation Using Unsupervised Learning (Mall Customers)

# 📌 Objective:
The objective of this project is to segment customers based on their spending behavior using unsupervised learning techniques. By identifying different customer groups, businesses can better understand purchasing patterns and design targeted marketing strategies for each segment. The dataset used for this task is the Mall Customers Dataset, which contains demographic and spending information of mall visitors.

# 📊 Dataset
The dataset contains information about mall customers such as:

Customer ID
Gender
Age
Annual Income (k$)
Spending Score (1–100)

The Spending Score is assigned by the mall based on customer behavior and spending patterns.

# 🛠️ Approach:

# 1️⃣ Exploratory Data Analysis (EDA)
The dataset was explored using Python libraries such as Pandas, Matplotlib, and Seaborn to understand the distribution of customer attributes and identify patterns in the data.

Key analyses included:

1) Age distribution of customers
2) Gender distribution
3) Relationship between annual income and spending score
4) Correlation between numerical variables

# 2️⃣ Customer Segmentation using K-Means
The K-Means clustering algorithm was applied to segment customers into distinct groups based on their income and spending behavior.

Steps included:

1) Selecting relevant features such as Annual Income and Spending Score
2) Determining the optimal number of clusters using the Elbow Method
3) Applying the K-Means algorithm to create meaningful customer segments

# 3️⃣ Cluster Visualization
To better visualize the clusters, dimensionality reduction techniques were applied:

PCA (Principal Component Analysis)
t-SNE (t-distributed Stochastic Neighbor Embedding)

These methods helped reduce the data to two dimensions and allowed the clusters to be visualized clearly through scatter plots.

# 4️⃣ Customer Segment Analysis
After clustering, each segment was analyzed based on its characteristics, such as income level and spending behavior. This helped identify different types of customers, for example:

1) High-income high-spending customers
2) High-income low-spending customers
3) Low-income high-spending customers
4) Low-income low-spending customers
5) Average customers

# 5️⃣ Marketing Strategy Recommendations
Based on the identified segments, targeted marketing strategies were proposed:

# 1) High Income – High Spending Customers

Offer VIP memberships and exclusive products
Provide personalized premium services

# 2) High Income – Low Spending Customers

Promote luxury products and personalized offers
Encourage engagement through exclusive discounts

# 3) Low Income – High Spending Customers

Offer promotional discounts and seasonal deals

# 4) Low Income – Low Spending Customers

Provide budget-friendly product bundles and clearance sales

# 5) Average Customers

Use loyalty programs and regular promotional campaigns

# 📈 Results and Findings:
The K-Means clustering algorithm successfully grouped customers into distinct segments based on their spending patterns. Visualization techniques such as PCA and t-SNE helped clearly illustrate the separation between clusters. The segmentation provides valuable insights that businesses can use to improve marketing strategies, enhance customer engagement, and increase revenue.

## Task 3: Energy Consumption Time Series Forecasting

# 📌 Objective:
The objective of this project is to forecast short-term household energy usage using historical patterns and time-based features. By predicting energy consumption, households and utility providers can optimize energy usage, reduce costs, and improve planning. The dataset used for this task is the Household Power Consumption Dataset, which contains detailed records of household electricity usage over time.

# 📊 Dataset
The dataset contains the following information:

Date and Time
Global Active Power (kilowatts)
Global Reactive Power
Voltage
Sub-metering readings (kitchen, laundry, heating, etc.)

The target variable for forecasting is:

Global Active Power → represents household energy consumption in kilowatts.

# 🛠️ Approach:

# 1️⃣ Time Series Parsing and Resampling

1) Combined the Date and Time columns into a single datetime column.
2) Converted the target variable to numeric type and handled missing values.
3) Resampled the data to hourly averages to create a consistent time series.

# 2️⃣ Feature Engineering

Extracted time-based features such as:

Hour of the day
Weekday vs. weekend indicator

These features help models capture temporal patterns and improve forecast accuracy.

# 3️⃣ Model Training and Comparison
Three different forecasting models were applied and compared:

# 1) ARIMA (Auto-Regressive Integrated Moving Average):

Captures linear temporal dependencies in the time series.

# 2) Prophet:

Designed for time series with strong seasonal patterns and missing data.

# 3) XGBoost Regression:

Uses time-based features as input to model non-linear patterns.

Models were evaluated using RMSE (Root Mean Squared Error) to compare prediction accuracy.

# 4️⃣ Forecast Visualization

Plotted actual vs. predicted energy usage for all models

Visualization helps assess the model’s performance over time and identify periods where forecasts deviate from actual consumption.

# 📈 Results and Findings

1) ARIMA effectively captured short-term linear trends in energy usage.
2) Prophet performed well in handling seasonal patterns and daily fluctuations.
3) XGBoost captured non-linear relationships using time-based features and often outperformed linear models in certain periods.
4) Combining feature engineering with appropriate forecasting models provides accurate predictions for household energy planning.
