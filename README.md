# Credit_Risk_Analysis

## Project Overview

This project involved the usage of Python and machine learning models to predict credit risk. The objective is to identify if a person will a high risk or a low risk candidate for the loan. We used a few different machine learning models and the goal is to evaluate the models based on the accuracy and make a recommendation on whether any of the models can be used to predict credit risk. 

The different models used are:
* RandomOverSampler
* SMOTE Oversampling
* Undersampling using the ClusterCentroids algorithm
* Combination (Over and Under) sampling using the SMOTEENN algorithm
* Random Forest Classifier
* Easy Ensemble Adaboost Classifier

## Resources
* [Loans Dataset](https://github.com/dkatragadda/Credit_Risk_Analysis/blob/main/Resources/LoanStats_2019Q1.csv "Loans Dataset")
* Tools Used: Python 3.7, Jupyter Notebook, Libraries - scikit learn, numpy, pandas etc. 

## Results

### RandomOverSampler model results

![RandomOverSamplerStats](https://github.com/dkatragadda/Credit_Risk_Analysis/blob/main/Resources/RandomOverSamplingStats.png)

The accuracy of this model is 66.5%. The precision for the high-risk loans is only 1% and the recall/sensitivity is 66% with an F1 score of 2%. Due to the larger sample size of low-risk loans, the precision is higher at 100% with a recall/sensitivity of 67% and an F1 score of 80%.

### SMOTE Oversampling model results

![SMOTEOversamplingStats](https://github.com/dkatragadda/Credit_Risk_Analysis/blob/main/Resources/SmoteOversamplingStats.png)

The accuracy of this model is 64.4%. The precision for the high-risk loans is only 1% and the recall/sensitivity is 61% with an F1 score of 2%. Due to the larger sample size of low-risk loans, the precision is higher at 100% with a recall/sensitivity of 64% and an F1 score of 78%.

### Undersampling using ClusterCentroids model results

![ClusterCentroidsStats](https://github.com/dkatragadda/Credit_Risk_Analysis/blob/main/Resources/UndersamplingStats.png)

The accuracy of this model is 43.5%. The precision for the high-risk loans is only 1% and the recall/sensitivity is 59% with an F1 score of 1%. Due to the larger sample size of low-risk loans, the precision is higher at 100% with a recall/sensitivity of 43% and an F1 score of 60%.

### Combination (Over and Under) sampling using SMOTEENN model results

![SMOTEENNStats](https://github.com/dkatragadda/Credit_Risk_Analysis/blob/main/Resources/OverAndUnderSamplingStats.png)

The accuracy of this model is 54.1%. The precision for the high-risk loans is only 1% and the recall/sensitivity is 69% with an F1 score of 1%. Due to the larger sample size of low-risk loans, the precision is higher at 100% with a recall/sensitivity of 54% and an F1 score of 70%.

### Random Forest Classifier model results

![RandomForestClassifier](https://github.com/dkatragadda/Credit_Risk_Analysis/blob/main/Resources/RandomForestClassifierStats.png)

The accuracy of this model is 90.8%. The precision for the high-risk loans is only 4% and the recall/sensitivity is 67% with an F1 score of 7%. Due to the larger sample size of low-risk loans, the precision is higher at 100% with a recall/sensitivity of 91% and an F1 score of 95%.

### Easy Ensemble Adaboost model results

![AdaboostStats](https://github.com/dkatragadda/Credit_Risk_Analysis/blob/main/Resources/EasyEnsembleClassifierStats.png)

The accuracy of this model is 94.3%. The precision for the high-risk loans is only 7% and the recall/sensitivity is 90% with an F1 score of 14%. Due to the larger sample size of low-risk loans, the precision is higher at 100% with a recall/sensitivity of 94% and an F1 score of 97%.


## Summary 

Based on the analysis conducted, we can see that all the different models work well in predicting the low risk loans. As we evaluated the different models, the ensemble techniques performed marginally better than the oversampling and undersampling techniques. However, the highest precision we obtained with the Adaboost classifier was only 7% for high risk loans which is not good enough in the real world as a lot of low risk loans are still wrongly identified as high risk loans. On the same lines, the recall/sensitivity of the Adaboost model indicates that we are able to accurately predict high-risk loans 90% of the time. In summary, I do not recommend any of the techniques to be used by the team to predict credit risk. 

