# Machine Learning Trading Bot

## Overview of the Analysis
* This analysis used a dataset of historical lending activity from a peer-to-peer lending services company to build a model that can identify the creditworthiness of borrowers. The analysis used a logistic regression model to make decision as  whether to approve or deny a credit application based on customer's  personal information.  

* The data had two groups of loans: `0` (healthy loan)  class  and  `1` (high-risk loan). The former eventually performed well, and the latter eventually defaulted. The goal is to use classification to correctly predict which of these two categories a loan application belongs to.
*  The original dataset  used to build the logistic regression model (Model 1)  had  total number of 77,536 loans. Out of these 75.036 loans performed well  and 2,500 loans  became high-resk loans.   Resampled dataset had 56,271 loans in each class and this was used to build  Model 2 . 
* Below are the stages of the machine learning process completed as part of this analysis:

  * Split the Data into Training and Testing Sets using  ```train_test_split()```

  * Created a model with ```LogisticRegression()```

  * Trained  the model with ```model.fit()```

  * Made predictions with ```model.predict()```

  * Evaluated  the model with ```balanced_accuracy_score()```, ```confusion_matrix()``` and ```classification_report_imbalanced()```


* Below are the methods used in this analysis:
  * Used  logistic regression assesses  multiple variables, such as an applicant's income, loan amount, debt_to_income ratio and number of accounts, to arrive at one of two answers: approve or deny the loan application.

  * Oversampled  the data for the minority class `1`  with  RandomOverSampler( ) to enhance the performance of the model; 

## Results

* Machine Learning Model 1:
  * Accuracy  score 0.95,  meaning that the model can detect 95% of  true positives and true negatives

  * Precision  score for `0` (healthy loan)  class was 1.00  and  for `1` (high-risk loan) class was 0.85,  meaning that  model is  detecting  85% of the loans that were actually going to default

  * Recall scores score for `0` (healthy loan)  class was 0.99  and  for `1` (high-risk loan) class was 0.91,  meaning that the model  correctly clasified 91%  of the truly high risk loans.



* Machine Learning Model 2:
  * Accuracy  score 0.99,;

  * Precision  score for `0` (healthy loan)  class was 1.00  and  for `1` (high-risk loan) class was 0.84

  * Recall scores score for `0` (healthy loan)  class was 0.99  and  for `1` (high-risk loan) class was 0.99,

## Summary

The results regarding accuracy of the minority class are actually mixed when comparing the classifiction reports generated from the predictions with the original data versus the predictions with the resampled data. 

First, the accuracy score is higher for the resampled data (0.99 vs 0.95), meaning that the model using resampled data was much better at detecting true positives and true negatives. 

The precision for the `1` (high-risk loan) labels  is marginally higher with the orignal data (0.85) versus the resampled data (0.84) meaning that the original data was slightly better at detecting the users that were actually going to default. 

In terms of the recall, however, the `1` (high-risk loan) class metric using resampled data was much better than the original dataset (0.99 vs 0.91). Meaning that the resampled data correctly clasified a higher percentage of the truly defaulting borrowers. 

All in, the model using resampled data was much better at detecting borrowers who are likely to default than  the model generated using the original, imbalanced  data. 

In this analysis  where the company's priority is  to build a less risky loan book, model 2 is recommended because it has better recall score  for  the '1` (high-risk loan) class than model 1 as it is correctly classfying 99% of the truly high risk loans.

#  Algorithmic Trading Bot
This is an analysis of ETF data stored in SQL database to establish the performance of a hypothetical fintech ETF that consists of four stocks. The analysis is presented through professionally styled and formatted interactive visualizations and a screenshot of the web application that I created by deploying my Jupyter notebook via the Voilà library. 

## Methodology and Approach

Used SQL queries with Python, Pandas, and hvPlot to analyze the performance of a single asset from the ETF

Used advanced SQL queries to optimize the efficiency of accessing data from the database.

Built the ETF portfolio by using SQL joins to combine all the data for each asset and then evaluated its performance.

## Libraries and Technologies Used

- Pandas library -  a Python library for data analysis. 

- SQLAlchemy -SQL library for Python

- hvPlot - visualization library. 

- Voilà library - to deploy the Juypter library as a web application

- Jupyter notebook

## ETF financial application deployed to the web
Below is the ETF analysis deployed as a web application:
![Actual Retuns vs Strategy Returns SVM model](https://github.com/Abillu/ChallengeM14_Upload/assets/126644613/c7d04591-3016-472d-a49a-284feadc9a91)
![Actual Retuns vs Strategy Returns 6 months training window](https://github.com/Abillu/ChallengeM14_Upload/assets/126644613/3815aa5b-52a3-444c-8b16-9c840ecb9be8)
![Actual Retuns vs Strategy Returns SMA windows changed](https://github.com/Abillu/ChallengeM14_Upload/assets/126644613/46abd336-b362-416e-b259-1bcea898b554)
![Best improved trading algorithm returns](https://github.com/Abillu/ChallengeM14_Upload/assets/126644613/736811bd-aa9a-42ab-b296-9ee9f6e7a47d)
![Actual Retuns vs Strategy Returns LR model](https://github.com/Abillu/ChallengeM14_Upload/assets/126644613/bdd54453-4df7-4224-a245-26b865a4a8e0)



---
