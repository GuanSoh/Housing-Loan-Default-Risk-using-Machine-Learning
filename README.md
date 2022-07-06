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

Dataset used in this research is [Lending Club Loan Data from Kaggle](https://www.kaggle.com/datasets/wordsforthewise/lending-club). The dataset contains 2260701 of instances and 151 features. However, this project only focus on housing loan but Lending Club Loan Data consists multiple types of loan data like car loan, Medical loan, etc. So, only housing loan data will be extract and use in this project. Finally, the instances available in this research is 14136. Meanwhile, the dataset faces data imbalanced issue. Proportion for default label is 33% and 67% for non-default label. 

## Data Preprocessing

The data preprocessing part include missing values handling, outlier treatment, remove features could cause data leakage. 

## Exploratory Data Analysis

Some insights that important to analysis have been shown in this part.

![alt text](https://github.com/GuanSoh/Housing-Loan-Default-Risk-using-Machine-Learning/blob/main/Image/EDA_grade.png)

The loan grades are evaluating by Lending Club based on those applicant’s trustworthiness. As we can see, those applicants been classifying as low grades 
have higher possibility to default.

![alt text](https://github.com/GuanSoh/Housing-Loan-Default-Risk-using-Machine-Learning/blob/main/Image/EDA_pub_rec.png)

Image above show that percentage of default increased as number of times the applicant involved in derogatory public record. This could be because those related applicants usually don’t have much responsibility for others.

![alt text](https://github.com/GuanSoh/Housing-Loan-Default-Risk-using-Machine-Learning/blob/main/Image/EDA_term.png)

Percentage of default for 60 months’ loan term is higher than those apply for 36 months’ loan term. This may because when the loan term longer, applicant money flow will be constraints by interest fee longer time which lead to less saving and need proper fund management. If any problem exists in their money flow again, for example like emergency, their available funds will be more limited.

## Models Traning and Testing

Logistic Regression, Support Vector Machine, Decision Tree and Random Forest been selected to perform classification in this project. Comparison been made to identify most accurate algorithm. Decision Tree been selected as baseline model since we can't find benchmark model for this research. 

![alt text](https://github.com/GuanSoh/Housing-Loan-Default-Risk-using-Machine-Learning/blob/main/Image/Performance%20of%20each%20models.png)

Support vector machine gets the highest f1-score and recall which is 77% and 90%. In the same time, baseline model decision tree only gets 66% of f1-score and 70% of recall.

![alt text](https://github.com/GuanSoh/Housing-Loan-Default-Risk-using-Machine-Learning/blob/main/Image/Model%20Performance%20between%20training%20and%20testing.png)

Image above show the performance of models in training set and testing set. Decision tree and random forest may face overfitting problem due to huge different result in training set and testing set. This may because these two algorithm are complex algorithm and the size of the dataset in this research is not enough for them.

![alt text](https://github.com/GuanSoh/Housing-Loan-Default-Risk-using-Machine-Learning/blob/main/Image/Model%20Performance%20between%20SMOTE%20and%20without%20SMOTE.png)

Lastly, the after applying SMOTE method to handling data imbalanced problem, each model’s precision are slightly decrease but f1-score increase slightly and recall is significantly increase. Especially for support vector machine, its recall increased from 74% to 90% which is total 19% of incensement. As recall for each models increased, which indicated each models perform better in detecting positives cases or minority cases. Therefore, with handling data imbalanced using SMOTE, each machine learning models perform better in detecting defaulter.

## Conclusion

In conclusion, support vector machine performs the best in this research, which gets 67% of precision, 90% of recall and 77% of f1-scores. Besides that, after applying SMOTE, each models perform better in detecting defaulter

## Remark

To get more details information about this project, can go through my [research paper](https://github.com/GuanSoh/Housing-Loan-Default-Risk-using-Machine-Learning/blob/main/Research%20Paper/Tong%20Gee%20Kok_1171103482_FYP2ResearchPaper.pdf)




