# Credit_Risk_Analysis
### Overview of the analysis :
#### Purpose of the analysis is to apply machine learning learning to solve a real-world challenge: credit card risk.Credit risk is an inherently unbalanced classification problem, as good loans easily outnumber risky loans. We Used the credit card credit dataset from LendingClub, a peer-to-peer lending services company,we  oversample the data using the RandomOverSampler and SMOTE algorithms, and undersample the data using the ClusterCentroids algorithm. And used a combinatorial approach of over- and undersampling using the SMOTEENN algorithm. We compare two new machine learning models that reduce bias, BalancedRandomForestClassifier and EasyEnsembleClassifier, to predict credit risk
#### Being able to predict credit risk with machine learning algorithms can help banks and financial institutions predict anomalies, reduce risk cases, monitor portfolios, and provide recommendations on what to do in cases of fraud.
#### Data used :
#### 2020Q1loans.csv
### Results:
#### Oversampling:
#### Naive Random Oversampling.
##### The accuracy score for the random oversampling is 0.63.The classification report is given as follows. The precision for high_risk is 0.01 and for low risk is 1.00 , very low and high for the low risk, indicating an overfitting for the low_risk. The recall socre for high risk is 0.62  and low risk is 0.65 is not ideal.
 is 0.65![image](https://user-images.githubusercontent.com/100485119/175836633-4b0442d0-57c4-49fe-a4bd-b84661beecbf.png)

#### SMOTE Oversampling
###### The balance accuracy score for the SMOTE oversampling is 0.66.The classification report is given as follows. The precision for high_risk is 0.01 and for low risk is 1.00 , very low and high for the low risk, indicating an overfitting for the low_risk. The recall socre for high risk is 0.63  and low risk is 0.69 is not ideal.
![image](https://user-images.githubusercontent.com/100485119/175836645-794a345a-d98b-4bed-993a-f1e3e19f7850.png)

#### Undersampling:
###### The balance accuracy score for the Undersampling is 0.63.The classification report is given as follows. The precision for high_risk is 0.01 and for low risk is 1.00 , very low and high for the low risk, indicating an overfitting for the low_risk. The recall socre for high risk is 0.63  and low risk is 0.69 is not ideal.
![image](https://user-images.githubusercontent.com/100485119/175836667-ae274c42-9077-4638-8b4e-7f75ec645c1f.png)

#### Combination (Over and Under) Sampling
###### The  balance accuracy score for the Combination (Over and Under) Sampling is 0.58.The classification report is given as follows. The precision for high_risk is 0.01 and for low risk is 1.00 , very low and high for the low risk, indicating an overfitting for the low_risk. The recall socre for high risk is 0.63  and low risk is 0.55 is not ideal.
![image](https://user-images.githubusercontent.com/100485119/175836679-4cbdebdc-6558-4a37-9e36-8a85b2329b61.png)

#### Balanced Random Forest Classifier
###### The  balanace accuracy score for the Balanced Random Forest Classifier is 0.78.The classification report is given as follows. The precision for high_risk is 0.04 amd low risk is 1.00, very low and high for the low risk, indicating an overfitting for the low_risk.  The recall socre for high risk is 0.67  and low risk is 0.91 is not ideal.
![image](https://user-images.githubusercontent.com/100485119/175836700-044bbd73-e926-4bad-a3f9-e1c4b21f2657.png)

#### Easy Ensemble AdaBoost Classifier
###### The  balanace accuracy score for the Easy Ensemble AdaBoost Classifier is 0.92.The classification report is given as follows. The precision for high_risk is 0.08 amd low risk is 1.00,   The recall socre for high risk is 0.91  and low risk is 0.94 is good.
![image](https://user-images.githubusercontent.com/100485119/175836718-1094e526-18d7-408b-ad2b-d4fef923c2dc.png)

### Summary:
#### Without scaling the data, the random forest classifier model is prodcuing the most accurate model at this point, defying my prediction. 
#### Easy Ensemble AdaBoost Classifier has the highest balance accuracy score. logistic regression model will perform better for this dataset
#### More detailed model to distinguish the features need to be establlished for a better prediction.
