# Credit-Card-Churn-Analysis

Predicting credit card users churn. Task is to help a bank predict who is likely to cancel their credit card by building and evaluating a classification model.

1. Exploratory Data Analysis (EDA)
2. Data Preparation
3. Model Building
4. Performance Evaluation
5. Model Selection

# Data Description
* CLIENTNUM: Client number. Unique identifier for the customer holding the account
* Attrition_Flag: Internal event (customer activity) variable - if the account is closed then "Attrited Customer" else "Existing Customer"
* Customer_Age: Age in Years
* Gender: Gender of the account holder
* Dependent_count: Number of dependents
* Education_Level: Educational Qualification of the account holder - Graduate, High School, Unknown, Uneducated, College(refers to college student), Post-Graduate, Doctorate
* Marital_Status: Marital Status of the account holder
* Income_Category: Annual Income Category of the account holder
* Card_Category: Type of Card
* Months_on_book: Period of relationship with the bank (in months)
* Total_Relationship_Count: Total no. of products held by the customer
* Months_Inactive_12_mon: No. of months inactive in the last 12 months
* Contacts_Count_12_mon: No. of Contacts in the last 12 months
* Credit_Limit: Credit Limit on the Credit Card
* Total_Revolving_Bal: Total Revolving Balance on the Credit Card
* Avg_Open_To_Buy: Open to Buy Credit Line (Average of last 12 months)
* Total_Amt_Chng_Q4_Q1: Change in Transaction Amount 
* Total_Trans_Amt: Total Transaction Amount (Last 12 months)
* Total_Trans_Ct: Total Transaction Count (Last 12 months)
* Total_Ct_Chng_Q4_Q1: Change in Transaction Count 
* Avg_Utilization_Ratio: Average Card Utilization Ratio

Model Building
During model evaluation in binary classification, there are two types of predictions that can be made incorrectly:

Type 1 Error (False Positive): This occurs when the model incorrectly predicts a positive outcome when the actual outcome is negative.

Type 2 Error (False Negative): This occurs when the model incorrectly predicts a negative outcome when the actual outcome is positive.

In the context of model evaluation for customer churn prediction, prioritizing recall over precision is paramount. Recall reflects the model's capacity to accurately detect all instances of customer churn, even if it results in some false alarms. Minimizing false negatives, where actual churn cases are missed, is crucial as it directly serves the business objective of retaining customers. This emphasis on recall may lead to an increase in false positives (incorrectly predicting churn), but it represents a strategic trade-off aimed at efficiently identifying and retaining customers at risk of churning.



# Logistic Regression Evaluation on Test Data
The logistic regression model, designed to predict credit card churn, exhibits an accuracy of 88% on both the training and testing datasets. However, its recall, which indicates the model's ability to identify customers at risk of attrition, is only 44%. This suggests that the model misses over half of potential churn cases, potentially impacting customer retention efforts. Further improvements or alternative models may be necessary to enhance performance.

Additionally, considerations such as calculating odds, precision-recall curve analysis, threshold calculation, and reevaluation on the test data may provide deeper insights into the model's performance and guide future refinement efforts.
