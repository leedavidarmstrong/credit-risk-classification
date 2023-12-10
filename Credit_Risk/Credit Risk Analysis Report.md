Credit Risk Analysis Report

## Overview of the Analysis
** MY ANSWER ** The purpose of this analysis was to develop and evaluate machine learning models capable of assessing credit risk based on financial data. 

In this section, describe the analysis you completed for the machine learning models used in this Challenge. This might include:

* Explain the purpose of the analysis.
** MY ANSWER ** The main goal was to predict the likelihood of loan default, which is crucial for any lending institution. The ability to accurately assess the risk associated with each loan helps in making informed lending decisions and in managing financial risks effectively.

* Explain what financial information the data was on, and what you needed to predict.
** MY ANSWER ** The dataset included several financial variables, such as loan size, interest rate, borrower income, debt-to-income ratio, number of accounts, derogatory marks, total debt, and the loan status. The key task was to predict the 'loan_status' - whether a loan would be healthy (0) or high-risk (1).

* Provide basic information about the variables you were trying to predict (e.g., `value_counts`).
** MY ANSWER ** The variable to predict was loan_status, with '0' indicating a healthy loan and '1' indicating a high risk of defaulting. A summary of value_counts for this variable would provide insights into the distribution of healthy and high-risk loans in the dataset.

* Describe the stages of the machine learning process you went through as part of this analysis.
** MY ANSWER ** The process involved data preprocessing (reading data, handling missing values, encoding categorical variables), splitting the data into training and testing sets, and then training and testing the machine learning models.

* Briefly touch on any methods you used (e.g., `LogisticRegression`, or any resampling method).
** MY ANSWER ** Logistic Regression was used as the primary method for this analysis. This choice was made due to its effectiveness in binary classification tasks, like predicting loan default (binary outcome: yes or no).

## Results

Using bulleted lists, describe the balanced accuracy scores and the precision and recall scores of all machine learning models.

* Machine Learning Model 1:
  * Description of Model 1 Accuracy, Precision, and Recall scores.
** MY ANSWER ** 
    . Accuracy: The model achieved an accuracy of 99%, which is exceptionally high and indicates a high level of overall correctness in its predictions.
    . Precision for Healthy Loans (0): 100%, showing excellent reliability in predicting low-risk loans.
    . Recall for Healthy Loans (0): 99%, indicating the model's ability to correctly identify the majority of low-risk loans.
    . Precision for High-Risk Loans (1): 85%, which is quite high and indicates the model's reliability in identifying loans at high risk of default.
    . Recall for High-Risk Loans (1): 91%, suggesting that the model can correctly identify a high percentage of high-risk loans.

## Summary

Summarise the results of the machine learning model, and include a recommendation on the model to use, if any. For example:
* Which one seems to perform best? How do you know it performs best?
** MY ANSWER ** The Logistic Regression model demonstrated strong performance in identifying both healthy and high-risk loans. Its high accuracy, combined with excellent precision and recall for healthy loans and good scores for high-risk loans, makes it a valuable tool for assessing credit risk. The high precision for healthy loans minimizes the risk of lending to default-prone borrowers, and the effective recall for high-risk loans assists in mitigating potential financial losses. It is recommended to utilize this model for credit risk assessment in a lending institution. The model's ability to accurately classify loans into low-risk and high-risk categories can significantly contribute to informed decision-making in the lending process. 

* Does performance depend on the problem we are trying to solve? (For example, is it more important to predict the `1`'s, or predict the `0`'s? )
** MY ANSWER ** For high-risk loans ('1's), accurate prediction is crucial to avoid financial losses, emphasizing the importance of high recall to identify most high-risk loans. Conversely, for healthy loans ('0's), high precision ensures low-risk loans are correctly identified, reducing unexpected defaults. This balance between predicting '1's and '0's should align with the lending institution's risk tolerance, financial goals, and market conditions.

If you do not recommend any of the models, please justify your reasoning.
