# Credit scoring algorithm and its implementation in production

Nhi Tran
Indiana University Bloomington
804 N Woodbridge Drive 
Bloomington,Indiana 47408,USA 
nytran@iu.edu

## ABSTRACT
A credit scoring algorithm is essential to help bank determine whether to authorize a loan to consumers. Most of the decision requires fast result and high accuracy in order to improve the bank customer satisfaction and profit. Choosing a correct machine learning algorithm will result in high accuracy in the prediction and the implementation and its API/ processing optimization of the algorithm will result in the fast service a bank can provide to its customers.

## KEYWORDS
machine learning, predict algorithm, classification, devops, optimization, api
## 1 INTRODUCTION
For every machine learning problem, there are normally two main areas that everyone focus on: which machine learning algorithms to use and how to run the machine learning code to serve its purpose.

Most of the time, machine makes predictions by learning and observing the data patterns from previous existing data with known results. Once the training is over, the machine learning code can then be applied to new data and predict the unknown results by applying the trained patterns. 
Once the code is completed, the next thing to do would be determining how to retrieve and apply the result of the prediction to a production application.


## 2 DESIGN

### 2.1 DATASET

We are utilizing an existing dataset on Kaggle to train and test algorithms and determine which algorithms would be the best to predict the probability of someone experiencing financial distress in the next two years [@fa18-523-83-credit-dataset]. 

Data description:

* RevolvingUtilizationOfUnsecuredLines: Total balance on credit cards and personal lines of credit except real estate and no installment debt like car loans divided by the sum of credit limits - percentage
* age
* NumberOfTime30-59DaysPastDueNotWorse: Number of times borrower has been 30-59 days past due but no worse in the last 2 years.
* DebtRatio: Monthly debt payments, alimony,living costs divided by monthy gross income � percentage
* MonthlyIncome: real
* NumberOfOpenCreditLinesAndLoans: Number of Open loans (installment like car loan or mortgage) and Lines of credit (e.g. credit cards)
* NumberOfTimes90DaysLate: Number of times borrower has been 90 days or more past due.
* NumberRealEstateLoansOrLines: Number of mortgage and real estate loans including home equity lines of credit
* NumberOfTime60-89DaysPastDueNotWorse: Number of times borrower has been 60-89 days past due but no worse in the last 2 years.
* NumberOfDependents: Number of dependents in family excluding themselves (spouse, children etc.)

Training population:150000
Testing population: 102000

### 2.2 DATA VISUALIZATION

### 2.3 DATA CLEANING

### 2.4 ALGORITHMS USED
Random Forest, XGBoost, LightGBM, Support Vector Machine, Logistic regression

### 2.5 RESULTA COMPARISON

## 3 IMPLEMENTATION
### 3.1 TECHNOLOGIES USED
*	Flask API - to allow the ability to pass attributes into production application and receive result in json
*	Docker - container
*	AWS EC2 - cloud server that will host all the code
*	Python - used to built algorithms
           	*  Panda
		*  Numpy
		*  Scikit-learn
		?   Etc.


## 4 RESULTS

### 4.1 DEPLOYMENT BENCHMARKS
### 4.2 APPLICATION BENCHMARKS

## 5 LIMITATIONS

# CONCLUSION

# ACKNOWLEDGEMENTS

# REFERENCES
All references can be found in 

