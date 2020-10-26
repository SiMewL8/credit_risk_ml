# Supervised Machine Learning
Predict credit risk with machine learning algorithms and help financial institutions predict anomalies, reduce risk cases, monitor portfolios.

A company in the FinTech industry has asked an aspiring Data Science Machine Learning expert to ascertain credit risk in their loans dataset. Python will be
the main method of translating our code, with various SciKit libraries, algorithms, and machine learning models. Some of the tasks are:

- Train and test models from a cleaned and pruned dataset
- Use popular machine learning models such as logistic regression, decision tree, random forest, and support vector machine algorithms and interpret results
- Devise methodology to compare the advantages and disadvantages of each supervised learning algorithm
- Research ensemble and resampling techniques to improve model performance

For this challenge, I used Python to build and evaluate several machine learning models to predict credit risk which help financial institutions
predict anomalies, reduce risk cases, monitor portfolios. In the FinTech industry, the reliance of Machine learning models generate insight on many questions 
and decisions. Here are the precision and recall scores for all the classifier tests:

```
Balanced Random Forest Classifier

                precision   recall      f1    |  accuracy_score
    high_risk      0.03      0.64      0.06   |  0.7688
    low_risk       1.00      0.90      0.94   |  

Easy Ensemble AdaBoost Classifier

    high_risk      0.07      0.90      0.14   |  0.9205
    low_risk       1.00      0.94      0.97   |  

Random Oversampling

    high_risk      0.01      0.62      0.02   | 0.6103
    low_risk       1.00      0.60      0.75   |    

SMOTE

    high_risk      0.01      0.64      0.02   | 0.6390
    low_risk       1.00      0.64      0.78   |

ClusterCentroids

    high_risk      0.01      0.54      0.01   | 0.4834
    low_risk       0.99      0.42      0.59   |

SMOTEENN

    high_risk      0.01      0.71      0.02   | 0.6553
    low_risk       1.00      0.60      0.75   |
```
The classification report visualizer displays the precision, recall, F1, and support scores for our models, but the focus is on our precision and 
recall(sensitivity) scores for our tested and predicted datasets. The balance between high precision and recall will yield many results, with correct
labeling. The accuracy score, on the other hand, describes how well the tested dataset compared to our predicted dataset. A higher accuracy score helps establish the better models.

For the low risk credit scores, a model like Balanced Random Forest Classifier poses the highest score between high precision and high recall,
however, the F1 score is better indicator of a balance between precision and recall, since the F1 score displays a low F1 score if both precision
and recall do not mesh well together. Considering that into account, we could surmise that Easy Ensemble AdaBoost Classifier would be a great balance
between high recall for both low and high credit risk, while a low score for precision for high risk leads to many false positives. And even the accuracy score for this model attests to the F1 score balance, boasting the highest score of 92%!



