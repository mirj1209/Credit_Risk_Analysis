# Credit_Risk_Analysis
Supervised Machine Learning and Credit Risk
## Overview of analysis
### Purpose
This project is mainly to explain how a machine learning algorithm is used in data analytics, explore and compare different models of machine learning.
## Results
### Naive Random Oversampling
![image](https://user-images.githubusercontent.com/104941338/189024459-08a3474a-7d4c-4909-9e7f-3157602c5522.png)
![image](https://user-images.githubusercontent.com/104941338/189024522-a2ec9ae9-2f78-4987-a1da-9cf167806f59.png)
![image](https://user-images.githubusercontent.com/104941338/189024628-770c9878-c481-4d1d-912b-c4a542e75fe8.png)
- Balanced accuracy score is 65.2%
- The precision for low risk loans is high with 100% and a sensitivity of 68% with an f1 score of 81%
- The precision for high risk loans is low with only 1% with a sensitivity of 62% and an f1 score of 2%
### SMOTE Oversampling
![image](https://user-images.githubusercontent.com/104941338/189025054-4d8da10b-194f-4530-b7b5-fd24d570f87d.png)
![image](https://user-images.githubusercontent.com/104941338/189025099-05479584-8396-4bd8-a4f4-ffd4876b626f.png)
![image](https://user-images.githubusercontent.com/104941338/189025147-d3fee328-464f-49af-b90a-5553ff20863d.png)
- Balanced accurcacy score is 62.4%
- The precision for low risk loans is 100% with a sensitivity of 66% and an f1 score of 80%
- The precision for high risk loans is 1% with a sensitivity of 59% and an f1 score of 2%
### Logistic Regression model with Undersampling
![image](https://user-images.githubusercontent.com/104941338/189025551-c9bc6f0e-ae82-449a-bf62-0079f95a6ce8.png)
![image](https://user-images.githubusercontent.com/104941338/189025592-e90f0894-f892-4648-bda1-6d2070e50180.png)
![image](https://user-images.githubusercontent.com/104941338/189025623-cd8fc740-b3dd-49e1-882a-9b7e7ee5dc45.png)
- Balanced accuracy score is 62.4%
- The precision for low risk loans is 100% with a sensitivity of 45% and an f1 score of 62%
- The precision for high risk loans is 1%% with a sensitivity of 61% and an f1 score of 1%
### SMOTEENN (Combination of Oversampling and Undersampling)
![image](https://user-images.githubusercontent.com/104941338/189025983-39ac1f99-5775-44ef-beb9-d678c984edfe.png)
![image](https://user-images.githubusercontent.com/104941338/189026029-85b614cb-9e6f-42e9-bf3c-c23a9522a4ba.png)
![image](https://user-images.githubusercontent.com/104941338/189026090-261012c2-89e2-4b76-9614-174da6c3d7ce.png)
- Balanced accuracy score is 52.9%
- The precision for low risk loans is 100% with a sensitivity of 58% and an f1 score of 73%
- The precision for high risk loans is 1% with a sensitivity of 70% and an f1 score of 2% 
### Balanced Random Forest Classifier
![image](https://user-images.githubusercontent.com/104941338/189023085-5a89ac69-6201-411d-b09d-157c27522858.png)
![image](https://user-images.githubusercontent.com/104941338/189023143-faba33c9-e75c-4dd2-9d11-955f299de896.png)
![image](https://user-images.githubusercontent.com/104941338/189023196-bbfc2220-2602-4624-98a0-16780871f98b.png)
- Balanced accuracy score is 78.8%
- The precision is low for high-risk loans with 4% with 67% sensitivity and an f1 score of 7%
- Due to lower number of false positives, the low-risk sensitivity is 91% with 100% presicion
### Easy Ensemble AdaBoost Classifier
![image](https://user-images.githubusercontent.com/104941338/189026706-07089c4a-468a-4af6-8101-bbe35ea27edf.png)
![image](https://user-images.githubusercontent.com/104941338/189026744-b5d63357-80c4-4108-a3e9-685e8b06f694.png)
![image](https://user-images.githubusercontent.com/104941338/189026800-93db0346-27ee-4a4a-8ccf-9acb6f9470e3.png)
- Balanced accuracy score is 92.5%
- The precision for low risk loans is 100% with a sensitivity of 94% and an f1 score of 97%
- The precision for high risk loans is 7%% with a sensitivity of 91% and an f1 score of 14%
## Summary
All models used to perform the credit risk analysis show weak precision when determining if a credit risk is high. The ensemble models brought improvement on the sensitivity of the high risk credits. The EasyEnsemble classifier model shows a recall of 92% so it detects almost all high risk credit. but with a low precision a lot of low risk credits are still falsely detected as high risk. Therefore, I wouldn't really recommend the bank to use any of these models to predict credit risk since they're quite inaccurate when wanting to deal with credit risk.

