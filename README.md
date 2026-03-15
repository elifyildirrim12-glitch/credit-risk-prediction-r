Credit Risk Prediction Using Machine Learning in R
Project Overview
This project focuses on predicting credit risk using machine learning techniques implemented in R. Credit risk assessment is an important task for financial institutions because it helps identify borrowers who may fail to repay their loans.
Using historical loan data, several classification models were developed to predict whether a borrower represents a good or bad credit risk.
The analysis includes data preprocessing, exploratory data analysis, model development, and performance evaluation.
Dataset
The analysis uses the German Credit Dataset, which contains financial information about loan applicants.
Dataset characteristics:
Number of observations: 1000
Number of variables: 20
Target variable: Credit Risk (Good / Bad)
Example variables include:
Age
Credit amount
Loan duration
Employment status
Savings account status
Checking account status
Housing status
These variables are used to predict the probability of loan default.
Exploratory Data Analysis
Exploratory Data Analysis (EDA) was conducted to understand the structure of the dataset and identify patterns between variables.
Several visualizations were generated including:
Age distribution
Loan amount distribution
Loan duration distribution
Credit risk comparison using boxplots
Correlation matrix for numerical variables
These visualizations help identify potential relationships between financial characteristics and credit risk.
Machine Learning Models
Three machine learning models were implemented in this project:
Logistic Regression
Logistic regression is a widely used statistical method for binary classification problems. It estimates the probability that a borrower belongs to a specific credit risk category.
Advantages:
Simple and interpretable
Commonly used in financial risk modeling
Decision Tree
Decision trees classify observations by splitting the dataset based on feature values.
Advantages:
Easy to interpret
Visual decision rules
Useful for financial decision-making
Random Forest
Random Forest is an ensemble learning algorithm that combines multiple decision trees to improve prediction accuracy.
Advantages:
Higher predictive performance
Reduced overfitting
Handles complex relationships in data
Model Evaluation
Model performance was evaluated using several metrics:
Accuracy
Precision
Recall
ROC Curve
AUC (Area Under the Curve)
These metrics allow comparison between models and help identify the most effective algorithm.
Results
The comparison of the three models shows that:
Logistic Regression provides a solid baseline model.
Decision Trees offer interpretable decision structures.
Random Forest achieves the highest predictive performance.
Random Forest performed best because it captures complex relationships within the dataset and reduces model variance.
Variable Importance
The Random Forest model identified several important predictors for credit risk:
Credit amount
Loan duration
Age
Account status
These variables significantly influence the probability that a borrower will default.
Project Structure
credit-risk-project
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
caret package
randomForest package
rpart package
ggplot2
pROC
Conclusion
This project demonstrates how machine learning techniques can be used to improve credit risk prediction.
Among the tested models, Random Forest provided the best performance. The results show that machine learning models can support financial institutions in making more accurate lending decisions and reducing financial risk.
