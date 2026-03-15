Credit Risk Prediction using Machine Learning in R
A machine learning project that predicts credit risk using financial and demographic information of loan applicants. The project applies multiple classification algorithms and evaluates their performance using standard machine learning metrics.
Project Overview
Credit risk assessment is a critical task for financial institutions. Incorrect credit decisions can lead to significant financial losses. Machine learning techniques allow financial institutions to analyze historical data and identify patterns that indicate whether a borrower is likely to default.
This project builds predictive models to classify loan applicants as good credit risk or bad credit risk using the R programming language.
Dataset
The analysis is based on the German Credit Dataset, which contains financial and demographic information about loan applicants.
Dataset characteristics:
1000 observations
20 variables
Target variable: Credit Risk Classification
Example variables:
Age
Credit Amount
Loan Duration
Employment Status
Savings Account Status
Checking Account Balance
Housing Status
Exploratory Data Analysis
Exploratory Data Analysis (EDA) was performed to understand the distribution of variables and identify relationships within the dataset.
The following visualizations were generated:
Age distribution
Credit amount distribution
Loan duration distribution
Credit risk comparison using boxplots
Correlation matrix of numerical variables
These visualizations help identify patterns that may influence credit risk prediction.
Machine Learning Models
Three classification models were implemented to predict credit risk.
Logistic Regression
Logistic regression is commonly used in credit risk analysis because it provides interpretable probability estimates.
Advantages:
Simple and interpretable
Widely used in financial modeling
Decision Tree
Decision trees classify observations by splitting the dataset based on feature values.
Advantages:
Easy to interpret
Provides visual decision rules
Random Forest
Random Forest is an ensemble learning algorithm that combines multiple decision trees to improve predictive performance.
Advantages:
Higher accuracy
Handles nonlinear relationships
Reduces overfitting
Model Evaluation
Model performance was evaluated using several metrics:
Accuracy
Precision
Recall
ROC Curve
AUC (Area Under the Curve)
These metrics allow comparison between models and help determine which algorithm performs best.
Results
The results show that:
Logistic Regression provides a reliable baseline model.
Decision Trees offer interpretable classification rules.
Random Forest achieves the highest predictive performance.
Random Forest performs best because it captures complex relationships within the dataset.
Variable Importance
The Random Forest model identified the most influential variables affecting credit risk prediction.
Important predictors include:
Credit amount
Loan duration
Age
Account status
These variables significantly influence the probability that a borrower will default.
Project Structure
credit-risk-prediction-r
│
├── data
│   └── dataset.csv
│
├── R
│   └── credit_risk_analysis.R
│
├── results
│   ├── model_results.csv
│   ├── roc_curves
│   └── feature_importance.png
│
└── README.md
Technologies Used
This project was implemented using the following tools:
R Programming Language
caret
randomForest
rpart
ggplot2
pROC
Conclusion
This project demonstrates how machine learning techniques can be applied to credit risk prediction.
The Random Forest model achieved the highest performance among the tested models. The results highlight the potential of machine learning methods to support financial institutions in making better lending decisions.
Author
Elif Yıldırım
Yeditepe University – Mathematics
