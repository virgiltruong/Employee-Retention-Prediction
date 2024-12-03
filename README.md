# Employee Retention Prediction
## Overview 

The goal of this project was to identify the factor that's likely to make employees leave the Salifort Motors. In doing so, I will use two approaches: Logistic Regression and Random Forest Machine Learning. The data set used in this project is the Human Resources (HR) data from Salifort Motors from [Kaggle](https://www.kaggle.com/datasets/mfaisalqureshi/hr-analytics-and-job-prediction?select=HR_comma_sep.csv). Based on the predictions of the Random Forest Model, the factors that affected an employee's decision most are their satisfaction level, number of projects assigned, and the time spent at the company (tenure).

## Business Understanding 

The HR department at Salifort Motors wants to take some initiatives to improve employee satisfaction levels at the company. They collected data from employees, but now they don’t know what to do with it. They refer to me as a data analytics professional and ask you to provide data-driven suggestions based on my understanding of the data. They have the following question: what’s likely to make the employee leave the company?

My goals in this project are to analyze the data collected by the HR department and to build a model that predicts whether or not an employee will leave the company.

## Data Understanding

The dataset that I'll be using in this project contains 15,000 rows and 10 columns for the variables listed below. 

**Note:** For more information about the data, refer to its source on [Kaggle](https://www.kaggle.com/datasets/mfaisalqureshi/hr-analytics-and-job-prediction?select=HR_comma_sep.csv).

Variable  |Description |
-----|-----|
satisfaction_level|Employee-reported job satisfaction level [0&ndash;1]|
last_evaluation|Score of employee's last performance review [0&ndash;1]|
number_project|Number of projects employee contributes to|
average_monthly_hours|Average number of hours employee worked per month|
time_spend_company|How long the employee has been with the company (years)
Work_accident|Whether or not the employee experienced an accident while at work
left|Whether or not the employee left the company
promotion_last_5years|Whether or not the employee was promoted in the last 5 years
Department|The employee's department
salary|The employee's salary (U.S. dollars)

## Modeling and Evaluation

### Logistic Regression:
  
  - Accuracy (0.82): The logistic regression model correctly predicted the target variable (whether an employee leaves or not) 82% of the time
  
  - Recall (0.82): The model correctly identified 82% of the employees who actually left the company, capturing a good portion of the positive cases.
  
  - Precision (0.79): 79% of the employees predicted to leave were correctly identified as leavers, indicating a relatively high number of false positives.
  
  - F1 Score (0.80): The logistic regression model does a decent job in balancing both false positives and false negatives.
        
### Random Forest:

  - Accuracy (0.99): The random forest model correctly predicted the target variable 99% of the time, which indicates excellent overall performance. However, such a high accuracy might suggest overfitting.
  - Recall (0.92): The random forest model identified 92% of the employees who left the company, indicating strong performance in detecting the positive class.
  - Precision (0.99): 99% of the employees predicted to leave were correctly identified as leavers, with very few false positives.
  - F1 Score (0.95): The random forest model is both highly accurate and reliable in identifying employees likely to leave.
