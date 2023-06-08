# Machine Learning Trading Bot

## Overview of the Analysis
* In this review aims to improve the existing algorithmic trading systems and maintain a firm’s competitive advantage in the market by  enhancing the existing trading signals with machine learning algorithms that can adapt to new data.



## Methodology and Approach

Implement an algorithmic trading strategy that uses machine learning to automate the trade decisions.

Adjust the input parameters to optimize the trading algorithm.

Train a new machine learning model and compare its performance to that of a baseline model.
## Libraries and Technologies Used

- Pandas library -  a Python library for data analysis. 

- TensorFlow and Keras libraries  - build deep learning model.

- sklearn library to train model and standardize data 

- Jupyter notebook
## EVALUATION REPORT 

Below is evaluation of the models:
Actual returns vs Strategy Returns using SVM model
![Actual Retuns vs Strategy Returns SVM model](https://github.com/Abillu/ChallengeM14_Upload/assets/126644613/c7d04591-3016-472d-a49a-284feadc9a91)

Actual returns vs Strategy Returns -training window increased to 6 months 
![Actual Retuns vs Strategy Returns 6 months training window](https://github.com/Abillu/ChallengeM14_Upload/assets/126644613/3815aa5b-52a3-444c-8b16-9c840ecb9be8)
The   training window was increased to 6 months from the inititial 3 months. This cumulative strategy returns were 180% compared to  returnss under the 3 months training window of ~150% . However during the period 2019 and 2020 the SVM model trading algorithim for the adjusted moel also made decisions that underperformed relative to the actual returns unlike in the original data set where the training algorithim largely overperfomerd relative to the actual returns

Actual returns vs Strategy Returns -2 days short SMA window , 150 days long SMA window
![Actual Retuns vs Strategy Returns SMA windows changed](https://github.com/Abillu/ChallengeM14_Upload/assets/126644613/46abd336-b362-416e-b259-1bcea898b554)
The short SMA window was dereased from 4 days to 2 days to two days and the lond SMA window was increased from 100 days to 150 days. This incerased the overall strategy returns to o~170% compared to the original  SMA windows returns of ~150% 

Best Improved trading algorithm 
![Best improved trading algorithm returns](https://github.com/Abillu/ChallengeM14_Upload/assets/126644613/736811bd-aa9a-42ab-b296-9ee9f6e7a47d)
The best improved SVM model was the one  with 6 months trading data and a  2 days SMA window and 150 days londg SMA window,. the SVM model returns were at 180% compared to the origina model . 

RLogistic Regression Model altertive
![Actual Retuns vs Strategy Returns LR model](https://github.com/Abillu/ChallengeM14_Upload/assets/126644613/bdd54453-4df7-4224-a245-26b865a4a8e0)

The logistical regression model model was compared to the orginal SVM model. The SVM moel perfomed better than the logistial model because the LR model made decisons in 2021 thats significantly underperformed relative to the actual returns. 




---
