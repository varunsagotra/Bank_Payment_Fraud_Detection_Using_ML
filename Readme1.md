Fraud Detection with Machine Learning On Banksim Payment Transaction Dataset - ( Dataset Name bs140513_032310)

Due to fraudulent transactions businesses lose millions of dollars each year and same behavior has been observed across many different fields such as e-commerce, UPI payment (digital banking), healthcare and regular banking systems.

Frauds can be detected via Automated detection system for that there are different approaches including rule based approaches and machine learning.
This repository uses the latter approach for classification of fraudulent transactions. The synthetically generated dataset consists of payments from various customers made in different time periods and with different amounts 
Below is a quick recap of the classification results of the machine learning models used in the script.

Insights observed using different modelling techniques ::

K-Neighbours Classifier ::
Classification Report for K-Nearest Neighbours: 
               precision    recall  f1-score   support

           0       1.00      0.98      0.99    176233
           1       0.98      1.00      0.99    176233

    accuracy                           0.99    352466
   macro avg       0.99      0.99      0.99    352466
weighted avg       0.99      0.99      0.99    352466

Confusion Matrix of K-Nearest Neigbours: 
 [[171999   4234]
 [   362 175871]]
 ******************************************************************************
 Random Forest Classifier ::
 Classification Report for Random Forest Classifier: 
                precision    recall  f1-score   support

            0       0.99      0.97      0.98    176233
            1       0.97      0.99      0.98    176233

     accuracy                           0.98    352466
    macro avg       0.98      0.98      0.98    352466
 weighted avg       0.98      0.98      0.98    352466

 Confusion Matrix of Random Forest Classifier: 
  [[170106   6127]
  [  1079 175154]]
 ******************************************************************************
 XGBoost Classifier ::
 Classification Report for XGBoost: 
                precision    recall  f1-score   support

            0       1.00      0.99      0.99    176233
            1       0.99      1.00      0.99    176233

     accuracy                           0.99    352466
    macro avg       0.99      0.99      0.99    352466
 weighted avg       0.99      0.99      0.99    352466

 Confusion Matrix of XGBoost: 
  [[174047   2186]
  [   706 175527]]
 ****************************************************************************** 

Original paper Reference is given below and also i have uploaded pdf (EMSS2014-Final) for your reference::

Lopez-Rojas, Edgar Alonso ; Axelsson, Stefan Banksim: A bank payments simulator for fraud detection research Inproceedings 26th European Modeling and Simulation Symposium, EMSS 2014, Bordeaux, France, pp. 144–152, Dime University of Genoa, 2014, ISBN: 9788897999324. https://www.researchgate.net/publication/265736405_BankSim_A_Bank_Payment_Simulation_for_Fraud_Detection_Research
