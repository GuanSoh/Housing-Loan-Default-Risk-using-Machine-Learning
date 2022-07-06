# Housing-Loan-Default-Risk-using-Machine-Learning
Final Year Project - Investigate machine learning models to classify housing loan defaulter before provide loan to them.

## Introduction

Loan interest fee if the core income for banking and lending institutions. Borrowers need to pay interest fee every month if applied loan from banking and lending institutions. However, loan default could happen and those institutions may lose their profits and funds.

Housing loan is one of the risky loan because it always involved huge amount of funds. Therefore, this project aim to minimize the loss of banking and lending institutions due to housing loan default by using machine learning. Meanwhile, data imbalanced is a data issue that always faced in loan default classification task which could limit the performance of models in detecting positive cases. So, this project will investigate the impact of Synthetic Minority Oversampling Technique (SMOTE) in handling data imbalanced issue.

## Objective for this project

1. To identify housing loan defaulter by using machine learning classification

2. To identify most accurate machine learning algorithms that train with provided housing loan default dataset by compare and evaluate their performance evaluation metrics.

3. To handle imbalanced data by using resampling algorithm.

## Dataset

Dataset used in this research is Lending Club Loan Data from Kaggle. The dataset contains 2260701 of instances and 151 features. However, this project only focus on housing loan but Lending Club Loan Data consists multiple types of loan data like car loan, Medical loan, etc. So, only housing loan data will be extract and use in this project. Finally, the instances available in this research is 14136. Meanwhile, the dataset faces data imbalanced issue. Proportion for default label is 33% and 67% for non-default label. 

## Data Preprocessing

The data preprocessing part include missing values handling, outlier treatment, remove features could cause data leakage. 

## Exploratory Data Analysis
