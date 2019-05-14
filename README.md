# Ad Click Prediction

This is a project aimed at predicting the probability of a  user clicking an ad displayed on the website. The dataset contains various features, including timestamp, website ID, browser information, offer ID, etc. pertaining to the advertisements displayed and the users' response. The challenge is to build a classification model that correctly predicts whether a user will click an ad, under various circumstances.

The primary issue with the dataset is that the Target feature is highly skewed with the number of negative samples being almost 100 times the number of positive samples available.We first try conventional approaches using various standard models, with the objective of achieving a high AUC score. The models that have been used include:

*   XGBoost
*   LightGBM
*   Random Forest Classifier

Following this, we follow two other approaches that are tailored to address the specific problem of the skewed dataset.

*   Logistic Regression with a custom cost function and gradient update rule
*   XGBoost with a modified dataset to counter skewness

