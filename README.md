# Approach to the Assignment
I have training and test dataset for binary classification problem. Training data 3910 records and 57 features. My job here is to do feature selection, preprocessing and finally train machine learning algorithm to predict the correct class.

Feature Selection
I have used mutual information as a measure of feature importance. Here I calculated mutual information of each feature with target variable to rank them.

Preprocessing
Data has no missing values, so that is sorted. I'm planning to use Random Forest for training so I can skip the scaling part as well. There slight class imbalance but not enough to worry about

Training
I have used random forest for training. I trained three versions. In first one I used all the features (57). In second version I used features selected (total 26 features) using Information gain. In third version I used features which had high mean accuracy decrease (14 features). I used third version as the final model for making predictions. all three models gave similar performance. I got the following results for the third model:

Accuracy: 95%
AUC-ROC: 0.99
F1 score: 0.95
