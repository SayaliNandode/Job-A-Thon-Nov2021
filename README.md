# Job-A-Thon-Nov2021

Approach to solve the problem
 
Problem Statement:
You are working as a data scientist with HR Department of a large insurance company focused on sales team attrition. Insurance sales teams help insurance companies generate new business by contacting potential customers and selling one or more types of insurance. The department generally sees high attrition and thus staffing becomes a crucial aspect.
To aid staffing, you are provided with the monthly information for a segment of employees for 2016 and 2017 and tasked to predict whether a current employee will be leaving the organization in the upcoming two quarters (01 Jan 2018 - 01 July 2018) or not, given:
1.	Demographics of the employee (city, age, gender etc.)
2.	Tenure information (joining date, Last Date)
3.	Historical data regarding the performance of the employee (Quarterly rating, Monthly business acquired, designation, salary)

Approach:
As the given problem is to predict whether a person will stay or not in the company, this is a binary classification problem.
As there are 10-11 features on which the output is to be predicted, the Decision Tree algorithm will give better results by calculating information gain at each step.
Steps performed as feature engineering/pre-processing are as follows:
1.     Calculated the tenor for which the person is present in the company.
2.     If the last working date is present in the dataset, that means the person has left the job. So, assigned the result as 1 for those employees and kept 0 for all other employees.
3.     One-Hot-Encoding is used for categorical variables in the dataset.
4.     Decision Tree Classifier is trained with gini index and entropy.
5.     Out of the 2 classifiers, the one with the gini index is giving better results, so this model is used further for testing the data.
6.     F1_Score is used as the metric to check performance of the model.

[Hackathon_Code_Approach.zip](https://github.com/SayaliNandode/Job-A-Thon-Nov2021/files/7576923/Hackathon_Code_Approach.zip)
