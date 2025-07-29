Project: Credit Repayment Prediction – Logistic Regression

The goal of this project was to build a classification model that predicts, based on client data, whether the client will repay a loan (1) or default (0). The analysis was based on demographic, financial, and occupational data.

The dataset included features such as age, number of children, marital status, place of residence, income, ownership of a bank account, credit card, or previous loans, as well as occupation, years of employment, and payment delinquency rate. All categorical variables were converted into numerical values using one-hot encoding.

The logistic regression model was trained on data split into training (70%) and testing (30%) sets. Its performance was evaluated using metrics such as accuracy, precision, recall, and F1-score.

Key factors influencing repayment prediction included primarily the absence of payment delays (which strongly reduces the risk of default), possession of a credit card, a bank account, and previous loans. Interestingly, certain occupations (e.g., salespeople) and specific employment statuses were associated with higher chances of repayment. Conversely, payment delays, lower education level, programmer occupation, being single, and residing in Wrocław were linked to a higher risk of default.

Results on the test set confirmed that the model effectively identifies clients who repay their loans (recall = 0.94), though it is somewhat less accurate in detecting defaulters (recall = 0.76). Overall model performance reached 87% accuracy and 86% macro F1-score.

In summary, logistic regression proved to be a solid model for predicting loan repayment. Future improvements could focus on better identifying high-risk clients through advanced feature engineering, optimizing the decision threshold, and testing more complex models such as random forests or XGBoost.

The model can be easily applied to predict single clients using the predict() and predict_proba() functions.
