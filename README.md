This project is related to the Online fraud In finanace. 
The Objective of this Project is detect the fraud . 
The dataset contains more than 6 lakhs rows. 
Most of columns is equal to zero.
The dataset is Imbalanced .


<=======================================================================CONCLUSION================================================================>
##### WITHOUT Handling imbalanced dataset:-
---------------------------------------------------------------------------------------------------------------------------------------------------
Best Model:- 
1. Decision Tree 
              precision    recall  f1-score   support

           0       1.00      1.00      1.00   1876979
           1       0.88      0.84      0.86      2443

    accuracy                           1.00   1879422
   macro avg       0.94      0.92      0.93   1879422
weighted avg       1.00      1.00      1.00   1879422

2. Random Forest :-
                precision    recall  f1-score   support

            0       1.00      1.00      1.00   1876979
            1       0.94      0.70      0.81      2443

    accuracy                           1.00   1879422
   macro avg       0.97      0.85      0.90   1879422
weighted avg       1.00      1.00      1.00   1879422

---------------------------------------------------------------------------------------------------------------------------------------------------
###### Handling Imbalaced Dataset
---------------------------------------------------------------------------------------------------------------------------------------------------
1. Undersampling:
Best Model:-
- Decision Tree:- Too Bad for precison and f1-score
                    precision    recall  f1-score   support

           0       1.00      0.99      0.99   1876979
           1       0.09      1.00      0.17      2443

    accuracy                           0.99   1879422
   macro avg       0.55      0.99      0.58   1879422
weighted avg       1.00      0.99      0.99   1879422
---------------------------------------------------------------------------------------------------------------------------------------------------
2. Oversampling 
Best Model:- 

- Decision Tree :-
                      precision    recall  f1-score   support

           0       1.00      1.00      1.00   1876979
           1       0.86      0.80      0.83      2443

    accuracy                           1.00   1879422
   macro avg       0.93      0.90      0.92   1879422
weighted avg       1.00      1.00      1.00   1879422
---------------------------------------------------------------------------------------------------------------------------------------------------
3. SMOTE
Best Model:-

- Decision Tree
              precision    recall  f1-score   support

           0       1.00      1.00      1.00   1876979
           1       0.61      0.97      0.75      2443

    accuracy                           1.00   1879422
   macro avg       0.81      0.99      0.88   1879422
weighted avg       1.00      1.00      1.00   1879422
---------------------------------------------------------------------------------------------------------------------------------------------------
4. Ensemble technique:

- BalancedRandomForestClassifier: Precision and F1-score is too bad
                precision    recall  f1-score   support

           0       1.00      0.98      0.99   1876979
           1       0.07      1.00      0.13      2443

    accuracy                           0.98   1879422
   macro avg       0.53      0.99      0.56   1879422
weighted avg       1.00      0.98      0.99   1879422

##### CONCLUSION
- The decision tree is working well for all cases . We can use decision tree models for predictions.
