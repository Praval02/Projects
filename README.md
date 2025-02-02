# Ttile: Diabetes Prediction System
## 1. Introduction
This project aims to predict the likelihood of a patient having diabetes using machine learning algorithms. The dataset used is the Pima Indians Diabetes Database, which contains various medical predictor variables and one target variable (diabetes outcome).
## 2. Description
The dataset consists of 768 instances of 9 features such as BMI, Glucose, Blood Pressure, Insulin, Age etc out of which some columns have outliers and missing values and one target variable named outcome having values either 0 or 1.
## 3. Methodology
### i) Data Preprocessing
First replaced enteries which are 0 to a form which can be treated as NULL by the compiler.
Analysed the data by studying boxplot and replaced null values with mean if number of outliers are less, else with median and also removed the column if majority of the values were missing.

Detected outliers using IQR method and replaced the enteries with lower bound and upper bound using capping

### ii) Training and Testing
Applied 5 classificiation algorithms namely Naive Bayes, K nearest neighbours, Random Forest, Logistic Regression and Decision Tree classifier and achieved maximum accuracy in case of Random Forest.

Further to crosscheck if accuracy can be improved further, applied Principle Component Analysis and applied same set of algorithms and there was no change in the accuracy rather it gave maximum accuracy in Logistic Regression

For both the cases, to check the best accuracy achieved, applied hyperpaprameter tuuning.
