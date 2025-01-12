# Predicting Loan Repayment or Default

This project aims to predict whether a loan will be repaid on time or default based on a set of features related to loan applicants. The dataset used includes information on past loans, detailing characteristics of 346 customers whose loans are either paid off or in default. The analysis uses machine learning algorithms such as K-Nearest Neighbors (KNN), Decision Trees, Support Vector Machine (SVM), and Logistic Regression to predict loan repayment status.

## Dataset

The dataset, `loan_train.csv`, contains the following fields:

| Field           | Description                                                              |
|-----------------|--------------------------------------------------------------------------|
| loan_status     | Whether a loan is paid off on time or in collection.                      |
| principal       | Basic principal loan amount.                                             |
| terms           | Origination terms (weekly, biweekly, or monthly payoff schedule).        |
| effective_date  | The date when the loan was originated.                                   |
| due_date        | The due date for loan repayment.                                          |
| age             | Age of the applicant.                                                    |
| education       | Education level of the applicant.                                        |
| gender          | Gender of the applicant.                                                 |

# Steps Involved

## Data Loading
- Load the dataset using pandas.

## Data Preprocessing
- Convert date columns to datetime objects.
- Handle categorical features such as gender and education.
- Feature engineering, including binarization of the weekend feature and one-hot encoding of education.

## Model Building
- Use various classification algorithms (KNN, Decision Tree, SVM, Logistic Regression) to predict loan repayment status.

## Model Evaluation
- Evaluate the models using accuracy metrics and confusion matrix.

# Data Visualizations
Visualize the loan repayment data:

- **Principal vs Loan Status**: Shows the relationship between loan principal amounts and loan status by gender.
- **Age vs Loan Status**: Visualizes age distribution for paid-off vs defaulted loans.
- **Day of the Week vs Loan Status**: Examines how loan repayment correlates with the day of the week.

# Machine Learning Models
The following machine learning algorithms were used:

- **K-Nearest Neighbors (KNN)**: To find the best k value and make predictions.
- **Decision Trees**: Used to build a tree-based model for loan repayment prediction.
- **Support Vector Machine (SVM)**: Applied to classify loan repayment status.
- **Logistic Regression**: Used to predict the likelihood of loan repayment.

The best-performing KNN model was selected based on accuracy.


