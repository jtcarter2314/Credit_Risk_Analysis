# Credit_Risk_Analysis

## Overview of the Analysis

In this procedure, we are using Python to use multiple machine learning models to predict credit risk. 
Models used:
- Oversampling
- Undersampling
- SMOTEENN algorithm using both oversampling and undersampling.
- Use of BalancedRandomForestClassifier and EasyEnsembleClassifier.

## Results

### RandomOverSampler Model

<img width="942" alt="Screen Shot 2021-11-05 at 8 43 16 PM" src="https://user-images.githubusercontent.com/86085982/140593719-3ef2099d-507b-4087-bd62-6e0b87b6f29a.png">

- The high_risk precision is about 1%, with 67% sensitivity which makes a F1 of 2%.

### SMOTE Model

<img width="942" alt="Screen Shot 2021-11-05 at 8 45 59 PM" src="https://user-images.githubusercontent.com/86085982/140593774-04d3756c-c9ed-4f36-928e-a9b8ddffc102.png">

- Results are similar.
- The balanced accuracy score is 65%.

### ClusterCentroids Cluster

<img width="942" alt="Screen Shot 2021-11-05 at 8 55 22 PM" src="https://user-images.githubusercontent.com/86085982/140593984-43fe7bbc-04e7-47db-ad53-7414cfd060e2.png">

Balanced accuracy score is down to about 51%.


### SMOTEENN model

<img width="942" alt="Screen Shot 2021-11-05 at 8 58 01 PM" src="https://user-images.githubusercontent.com/86085982/140594038-96d1a645-645a-4987-b0a9-c40db17c5c7b.png">

- the balanced accuracy score is about 62%.


 ### BalancedRandomForestClassifier model

<img width="942" alt="Screen Shot 2021-11-05 at 9 02 34 PM" src="https://user-images.githubusercontent.com/86085982/140594171-09df985f-b72f-44c1-8a4d-e57cc6001466.png">

- the balanced accuracy score is about 79%.

### EasyEnsembleClassifier model

<img width="942" alt="Screen Shot 2021-11-05 at 9 04 48 PM" src="https://user-images.githubusercontent.com/86085982/140594225-d420355a-1798-4c41-8e68-e29b258e0506.png">

- the balanced accuracy score is now rounded about to 93%.

## Summary

- The models show that the relation of the credit risk analysis show that it has a weak precision if a credit risk is high.
- EasyEnsembleClassifier shows a 93% that is almost all high risk credit. Though, if you pay attention to the low precision, low risk is detected incorrectly which negatively effects banks credit strategy and negates revenue. The best recommendation would be for the bank to not use the models to predict credit risk. 
