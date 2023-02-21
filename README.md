# Capstone

## Udacity Machine Learning Engineer Nanodegree

### Capstone Project

## Project: Predicting Loan Default for Lending Club

This is my independent final project for the Udacity Machine Learning Engineer Nanodegree.

The project requires Python and the following libraries:
-	NumPy
-	Pandas
-	Matplotlib
-	Seaborn
-	Scikit-learn

The repository includes: the project proposal (proposal.pdf), the project final report (capstone_report.pdf) and the Python code in jupyter notebook (capstone.ipynb).

### Data
The Lending Club data contain personal and financial information of borrowers together with their loan status, for the years 2007-2015.
The data can be downloaded from [Kaggle repository](https://www.kaggle.com/wendykan/lending-club-loan-data).

There are more than 880000 points and 73 features (list and description of features are reported at the beginning of the jupyter notebook).

The target variable is: ‘loan_status’. This column is used in the project to create a simpler binary target of good (0) and bad (1) loans.

### Project Overview
In this project, supervised learning techniques are applied on Lending Club data to identify borrowers who will not be able to pay back their loan. Data from past loans are used to train different classification models, which are evaluated in terms of accuracy, precision and especially recall. Imbalanced data are expected to pose a challenge for model performance.

The project proposal and the final report provide a thorough discussion of domain background, project aims, design, methodology, conclusions and ideas for further testing. 

The jupyter notebook contains several sections:
-	Importing libraries
-	Reading the data (with basic data exploration)
-	Exploratory data analysis
-	Data pre-processing
-	Separation between feature matrix and target
-	Splitting data into training and testing datasets
-	Feature scaling
-	Building and evaluating 4 different models with default hyperparameters (Gaussian Naïve Bayse, Logistic Regression, Random Forest Classifier, AdaBoost Classifier)
-	Optimisation of the models by using/tuning different hyperparameters or by over-sampling data using SMOTE algorithm.

The best result was obtained with an optimised Random Forest Classifier. This provided an accuracy of 0.97, a precision of 0.99 and a recall of 0.66. More research into dealing with imbalanced data (for example better use of SMOTE algorithm) and more testing of other type of models (for example XGBOOST or lightGBM) would be required to try to improve results, especially recall.
