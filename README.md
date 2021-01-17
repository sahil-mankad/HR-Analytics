# HR-Analytics

## Problem Statement: 
Your client is a large MNC and they have 9 broad verticals across the organisation. One of the problem your client is facing is around identifying the right people for promotion  and prepare them in time. The company needs help in identifying the eligible candidates at a particular checkpoint so that they can expedite the entire promotion cycle. They have provided multiple attributes around Employee's past and current performance along with demographics. Now, the task is to predict whether a potential promotee at checkpoint in the test set will be promoted or not after the evaluation process. This is a binary classification task wherein we have to predict if employee can be promoted or not.

## Contest Link: 
https://datahack.analyticsvidhya.com/contest/wns-analytics-hackathon-2018-1/

## Deploying the model locally
I have also added the code to deploy the model locally as a simple webpage, which is a form to collect details and predict outcome based on it. All the files neede are present in the Model Deployment folder. Download the dependencies given in below section, fire up your command prompt,change directory to the Model Deployment folder and run the below command

streamlit run deploy.py

Enter the details on web page, click on the predict button and voila, you'll get the prediction.

## Dependencies to install:

The jupyter notebooks were all executed in google colab. You will be able to see cells for where I have installed dependencies in colab, one of the examples is: 
! pip install catboost 
If you run the statement in colab it installs the library in colab. If you want to run it on your local pc, use pip install in your command prompt.
For the model deployment part, the dependencies can be installed as follows:

!pip install -q pyngrok

!pip install -q streamlit

!pip install -q streamlit_ace

!pip install pickle

! pip install catboost


## Details about each of the project files
I have used 3 notebooks as a part of this solution.
1. Eda HR Analytics.ipynb, where I've done detailed exploratory data analysis in order to gather some insights.
2. HR Analytics Modelling.ipynb, where tasks such as data pre-processing, feature engineering, modelling, ensembling and hyperparameter tuning have been taken care of. 
3. HR Analytics - Final Prediction.ipynb: This is where we first pre-process and engineer the features in test data, in a similar manner to that of train data and then used the best performing models in HR Analytics Modelling.ipynb notebook to predict the outcome for test data.

You can go through the notebooks one by one for more detailed analysis.

There are 3 data files:
1. train.csv: Training data
2. test.csv: Test data
3. sample_submission.csv: Examples of how the final outcome for submission should be like. 

I have also added the code for model deployment using streamlit in the repository in the folder named model deployment. This consists of the trained catboost classifier as a .pkl file,the deploy.py file which has the code for deploying app and the session state.py file which will help you create a session for your app. You can also find it here: https://drive.google.com/file/d/1D1HLyHfCAY2Bt0aVMFHVlLsSg4mUkon-/view. This will help you create a local app for the model.


