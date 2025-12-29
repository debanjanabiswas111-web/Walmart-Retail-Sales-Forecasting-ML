🛒 Retail Sales Machine Learning Project
📌 Project Overview

This project applies machine learning techniques to a real-world retail dataset to analyze and model weekly sales performance across multiple stores.

The project focuses on:

Regression – predicting exact weekly sales

Classification – identifying high vs low sales weeks

It is designed as an entry-level Data Science portfolio project, emphasizing clean code, proper ML methodology, and data-driven insights.

🎯 Business Problem

Retail businesses rely on sales forecasts to:

Plan inventory

Allocate staff

Optimize promotions

This project explores:

Which factors actually drive weekly sales, and how well can machine learning models predict them?

📂 Dataset

The dataset contains historical weekly sales data along with economic and store-level features.

Key Columns

Store – Store identifier

Date – Week of sales

Temperature

Fuel_Price

CPI – Consumer Price Index

Unemployment

Holiday_Flag – Indicates whether the week contains a major holiday

Weekly Sales – Target variable

🛠️ Tech Stack

Python

Pandas, NumPy

Matplotlib, Seaborn

Scikit-learn

Jupyter Notebook

🔄 Project Workflow
1️⃣ Data Understanding & Cleaning

Inspected dataset structure and column consistency

Standardized column names

Explicitly defined the target variable

Checked for missing values

2️⃣ Exploratory Data Analysis (EDA)

Analyzed sales distribution

Compared holiday vs non-holiday weeks

Examined correlations between economic indicators and sales

While holidays appeared to influence sales visually, further modeling showed their effect was weaker than expected.

3️⃣ Feature Engineering

Converted dates into:

Year

Month

Week number

Encoded categorical variables (Store)

Prepared data for both regression and classification tasks

🤖 Models Implemented
🔵 Regression Models (Predict Weekly Sales)
Model	Purpose
Linear Regression	Baseline model
Random Forest Regressor	Captures non-linear relationships

Evaluation Metrics

MAE (Mean Absolute Error)

RMSE (Root Mean Squared Error)

R² Score

🔍 Key Regression Insight

Random Forest significantly outperformed Linear Regression, indicating strong non-linear patterns in the data.

Feature importance analysis revealed:

Store was the dominant predictor

Economic indicators (CPI, Unemployment) were more influential than weather or holiday flags

Holiday_Flag had minimal importance once store and time-based features were included

🟢 Classification Models (High vs Low Sales)

Weekly sales were converted into a binary target:

1 → High Sales (above median)

0 → Low Sales (below median)

Model	Purpose
Logistic Regression	Interpretable baseline classifier
Decision Tree Classifier	Captures non-linear decision rules

Evaluation Metrics

Accuracy

Precision, Recall, F1-score

Confusion Matrix

📊 Key Results & Insights

Store-level patterns explain most of the variation in sales

Economic conditions matter more than short-term weather changes

Holiday effects are either weak or already captured by time-based features (week/month)

Tree-based models provide better performance and interpretability than linear baselines

Important Insight:
Although holidays are often assumed to strongly impact sales, feature importance analysis showed that Holiday_Flag contributed very little once store identity and temporal features were included.

📈 Feature Importance

Random Forest feature importance analysis showed:

Store (dominant)

CPI

Unemployment

Week of year

Binary features such as Holiday_Flag ranked near zero, highlighting the importance of validating assumptions with data.

🔮 Future Improvements

Hyperparameter tuning

Permutation feature importance

Cross-validation

Time-series forecasting (ARIMA / Prophet)

Deployment using Streamlit

💼 Why This Project Is Valuable

✔ Real-world dataset
✔ End-to-end ML workflow
✔ Multiple model comparison
✔ Honest, data-driven conclusions
✔ Strong interview discussion potential

🙋 About Me

Aspiring Data Scientist with a focus on applying machine learning to real-world business problems.
This project demonstrates my ability to analyze data critically, build models correctly, and interpret results beyond surface-level assumptions.
