# Project-Predicting-Credit-Card-Default

Team 1: Adil A Kumar, Daniel Byun, Ivy Zhou, Jiaqi Chen
1)	Business problem: Credit card companies primarily earn their money in three ways. They charge merchants a small % of every transaction made using their credit card. They charge customers interest on unpaid balance carried from month to month. They charge a variety of fees, including annual and late fees. When a customer is not able to pay bills by the due date and if the bank is certain they are not able to collect the payment, it will usually try to sell the loan. After that, if the bank recognizes that they are not able to sell it, they will write it off. This results in significant financial losses to the bank on top of the damaged credit rating of the customer and thus it is an important problem to be tackled. 
2)	Business Value: A credit card company based in Taiwan is looking to increase their profits. The company has identified an increasing trend of credit card payment defaults. The company wants to find out the likelihood of payment default for its customers and identify the important factors that determine credit card payment default. 
3)	Use case: The model could help the company decide which customers are high risk. High risk customers are those who run the risk of not paying off their bills. It would also help the company gain a deeper understanding of their current customers, which can channel future strategy, including offering targeted credit products to their customers.
4)	Data Science problem: Predict the probability of credit card default on payment next month for a customer.
The problem is a classification problem. Thus, it is a supervised learning problem.
5)	Data instance: Each row of data indicates a customer and their attributes. Below is a data snapshot along with data description.
 
 
Variable	Description
ID	Customer ID
LIMIT_BAL	Credit card limit
Sex	1=male, 2=female
Education	1=graduate school, 2=university, 3=high school, 4=others
Marriage	1 = married; 2 = single; 3 = others
Age	Customer age in years
PAY_0 – PAY_6	Past payment history status from September to April 2005
 -2 = no amount due, -1 = pay duly, 0 = revolving credit, 1-8 = payment delay for 1-8 months

BILL_AMT1-6	Credit card bill amount from September to April 2005
PAY_AMT1-6	Previous month amount paid from September to April 2005
default payment next month	Target Variable (1=yes, 0=no)

6)	Useful features: All columns in data look like useful features for modeling. However, since many of the columns are similar (ex: bill payment for successive months), there maybe a problem of multicollinearity. Exploratory data analysis may help in choosing the right variables for modeling. We may have to also create some new variables.
7)	Data Source - https://archive.ics.uci.edu/ml/datasets/default+of+credit+card+clients
The default of credit card clients Data Set is taken from the UCI machine learning repository. The dataset was collected for research purposes and captures credit card payment history in Taiwan for the period April – Sep 2005.
8)	Data input in python:
 
9)	Data instance count: 30000 rows and 25 columns
 
10)	Data Structure – 1 ID column, 23 Independent variables, 1 Target Variable
11)	Target variable class distribution –No (77.88%) , Yes (22.12%)
 
