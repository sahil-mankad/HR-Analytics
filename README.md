# HR-Analytics

Problem Statement: Your client is a large MNC and they have 9 broad verticals across the organisation. One of the problem your client is facing is around identifying the right people for promotion  and prepare them in time. The company needs help in identifying the eligible candidates at a particular checkpoint so that they can expedite the entire promotion cycle. They have provided multiple attributes around Employee's past and current performance along with demographics. Now, the task is to predict whether a potential promotee at checkpoint in the test set will be promoted or not after the evaluation process. This is a binary classification task wherein we have to predict if employee can be promoted or not.

Contest Link: https://datahack.analyticsvidhya.com/contest/wns-analytics-hackathon-2018-1/


I have used 3 notebooks as a part of this solution.
1. Eda HR Analytics.ipynb, where I've done detailed exploratory data analysis in order to gather some insights.
2. HR Analytics Modelling.ipynb, where tasks such as data pre-processing, feature engineering, modelling, ensembling and hyperparameter tuning have been taken care of. 
3. HR Analytics - Final Prediction.ipynb: This is where we first pre-process and engineer the features in test data, in a similar manner to that of train data and then used the best performing models in HR Analytics Modelling.ipynb notebook to predict the outcome for test data.

You can go throught the notebooks one by one for more detailed analysis.

There are 3 data files:
1. train.csv: Training data
2. test.csv: Test data
3. sample_submission.csv: Examples of how the final outcome for submission should be like. 
