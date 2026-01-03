Customer Churn Prediction Model
📌 Project Overview

This project focuses on building and evaluating a classification model to predict customer churn (whether a customer is likely to exit). The objective is to help businesses proactively identify at-risk customers and support data-driven retention strategies.

The model is trained on a structured banking dataset and evaluated using multiple performance metrics, probability thresholds, and visual diagnostics.

🗂 Dataset

Source: Bank churn dataset (≈80,000 records)

Target Variable: churn (customer exit indicator)

Features:

Demographic attributes

Account and financial indicators

Customer activity metrics

🔧 Data Preparation

Loaded and cleaned the dataset using a custom wrangling function

Removed non-numeric and irrelevant columns

Handled missing values

Separated features (X) and target (y)

Performed a train–test split to ensure unbiased evaluation

🧠 Modeling Approach

Trained a classification model to predict churn

Used probability outputs (predict_proba) for deeper insight beyond binary predictions

Evaluated model behavior across different decision thresholds

📊 Model Evaluation

The model was assessed using:

Confusion Matrix

True Positives

True Negatives

False Positives

False Negatives

Prediction Probability Distribution

Threshold Analysis

Compared model performance at multiple probability cutoffs (e.g. 0.3, 0.5, 0.7)

Demonstrated trade-offs between recall and precision

📈 Visualizations

Confusion Matrix plot for classification accuracy

Probability distribution of predicted churn likelihood

Threshold-based summary visualization to support business decision-making

🧾 Key Insights

The model effectively distinguishes between churned and retained customers.

Lower thresholds increase churn detection (recall) but raise false positives.

Higher thresholds improve precision but risk missing potential churners.

Threshold selection should align with business goals (e.g., aggressive retention vs cost control).

🛠 Tools & Technologies

Python

pandas

NumPy

scikit-learn

matplotlib

Jupyter Notebook

This churn prediction model enables organizations to:

Identify high-risk customers early

Optimize customer retention campaigns

Balance operational cost vs customer lifetime value

Support strategic decisions with interpretable analytics
