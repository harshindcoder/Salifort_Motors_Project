# Salifort Motors Project

## Overview
The goal of the project is to predict whether an employee will leave the company, and discover the reasons behind their departure, they could better understand the problem and develop a solution. Currently, there is a high rate of turnover among Salifort employees. (Note: In this context, turnover data includes both employees who choose to quit their job and employees who are let go). Salifort’s senior leadership team is concerned about how many employees are leaving the company. Salifort strives to create a corporate culture that supports employee success and professional development. 

## Business Understanding
The high turnover rate is costly in the financial sense. Salifort makes a big investment in recruiting, training, and upskilling its employees. If Salifort could predict whether an employee will leave the company, and discover the reasons behind their departure, they could better understand the problem and develop a solution.

## Data Understanding
This project uses a dataset called HR_capstone_dataset.csv. It represents 10 columns of self-reported information from employees of a multinational vehicle manufacturing corporation. 
The dataset contains:
14,999 rows – each row is a different employee’s self-reported information
10 columns
| Column Name              | Type     | Description                                                |
|--------------------------|----------|------------------------------------------------------------|
| satisfaction_level        | int64    | The employee’s self-reported satisfaction level [0-1]      |
| last_evaluation           | int64    | Score of employee's last performance review [0–1]          |
| number_project            | int64    | Number of projects employee contributes to                 |
| average_monthly_hours     | int64    | Average number of hours employee worked per month          |
| time_spend_company        | int64    | How long the employee has been with the company (years)    |
| work_accident             | int64    | Whether or not the employee experienced an accident while at work |
| left                      | int64    | Whether or not the employee left the company               |
| promotion_last_5years     | int64    | Whether or not the employee was promoted in the last 5 years |
| department                | str      | The employee's department                                  |
| salary                    | str      | The employee's salary (low, medium, or high)               |

## Modeling and Evaluation 

### Logistic Regression
The logistic regression model achieved precision of 80%, recall of 83%, f1-score of 80% (all weighted averages), and accuracy of 83%, on the test set.

### Tree-based Machine Learning
After conducting feature engineering, the decision tree model achieved AUC of 93.8%, precision of 87.0%, recall of 90.4%, f1-score of 88.7%, and accuracy of 96.2%, on the test set. The random forest modestly outperformed the decision tree model.

## Conclusion
The models and the feature importances extracted from the models confirm that employees at the company are overworked.

To retain employees, the following recommendations could be presented to the stakeholders:

* Cap the number of projects that employees can work on.
* Consider promoting employees who have been with the company for atleast four years, or conduct further investigation about why four-year tenured employees are so dissatisfied.
* Either reward employees for working longer hours, or don't require them to do so.
* If employees aren't familiar with the company's overtime pay policies, inform them about this. If the expectations around workload and time off aren't explicit, make them clear.
* Hold company-wide and within-team discussions to understand and address the company work culture, across the board and in specific contexts.
* High evaluation scores should not be reserved for employees who work 200+ hours per month. Consider a proportionate scale for rewarding employees who contribute more/put in more effort.

