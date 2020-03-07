# User_Retention_Analysis
The goal of the project is to analyze the existing user base in one of the health apps my consulting company built and segment them into groups that predict user activity, and then construct a predictive model to assess parameters that most likely contribute to user activity prediction. For security reasons, I cannot put data here.

## First Step
The first file '1.User_Login_Data_Visualization.ipynb' reads user login data from 'UserLog.csv', organizes it, and extracts features from this time series data to be used in later clustering step.

## Second Step
The second file '2. Cluster users based on user activity.ipynb' takes features extracted from user login data, combined the number of events the users attended to cluster users.

## Third Step
The third file '3. Build a predictive Model to assess feature importance.ipynb' build a predictive model to assess feature importance. The label of the users is from step 2, result of clustering users. The features used in this model includes user demography from 'userinfo.csv' and third party health data from smartphones and smart watches. Different models are compared, and Random Forest performs the best. So I use it to further assess feature importance.
Now when a new user log in the app and the company get the third party health data of the users, company can send customized notifications according to the values of the important features to potential low-activity users to optimize their engagement.

## Authors

* **Zhenru Zhou** 
