# Credit_Risk_Analysis

## Overview
Credit risk is an inherently unbalanced classification problem, as good loans easily outnumber risky loans. Through the use of machine learning, and several techniques under the overaching model of unsupervised learning, we employee several methods to analyze factors to predict credit risk within a dataset. Using the credit card credit dataset from LendingClub, a peer-to-peer lending services company, we've oversampled the data using the RandomOverSampler and SMOTE algorithms, and undersample the data using the ClusterCentroids algorithm. Then, we use a combinatorial approach of over- and undersampling using the SMOTEENN algorithm. Next, we compare two new machine learning models that reduce bias, BalancedRandomForestClassifier and EasyEnsembleClassifier, to predict credit risk. All these tasks were achieved with help from the imbalanced-learn and scikit-learn libraries to build and evaluate models using resampling.

## Results
### Naive Random Oversampling
<img width="725" alt="1_NaiveRandomOversampling" src="https://user-images.githubusercontent.com/95504135/165002795-942388d7-742f-4a30-a1ac-d786519d4b69.png">

* Balanced Accuracy: 0.63
* Precision: Low precision for High-risk loans and High precision for Low-risk loans
* Recall: 0.63 / 0.67

### SMOTE Oversampling
<img width="727" alt="2_SMOTE_Oversampling" src="https://user-images.githubusercontent.com/95504135/165002799-b6ae60ae-60c4-46db-bba8-2807f67e2f84.png">

* Balanced Accuracy: 0.55
* Precision: Low precision for High-risk loans and High precision for Low-risk loans
* Recall: 0.55 / 0.66

### Undersampling
<img width="724" alt="3_Undersampling" src="https://user-images.githubusercontent.com/95504135/165002803-4ce2e687-4493-4b93-95e3-8947a6c81dce.png">

* Balanced Accuracy: 0.57
* Precision: Low precision for High-risk loans and High precision for Low-risk loans
* Recall: 0.57 / 0.47

### Combination (Over and Under) Sampling
<img width="723" alt="4_CombinationOverUnderSampling" src="https://user-images.githubusercontent.com/95504135/165002804-9cce73e7-628b-4512-9d34-5e84403bbf69.png">

* Balanced Accuracy: 0.58
* Precision: Low precision for High-risk loans and High precision for Low-risk loans
* Recall: 0.70 / 0.58

### Forest Classifier
<img width="728" alt="5_ForestClassifier" src="https://user-images.githubusercontent.com/95504135/165002811-7343aa3d-147e-4908-a6e3-87b32d1c6064.png">

* Balanced Accuracy: 0.67
* Precision: Low precision for High-risk loans and High precision for Low-risk loans
* Recall: 0.67 / 0.91


### Easy Ensemble Ada Boost Classifier
<img width="730" alt="6_EasyEnsembleAdaBoostClassifier" src="https://user-images.githubusercontent.com/95504135/165002816-09c311f5-b14e-4157-84de-04fc6adfbbe5.png">

* Balanced Accuracy: 0.91
* Precision: Low precision for High-risk loans and High precision for Low-risk loans
* Recall: 0.91 / 0.94


## Summary
Throughout the several methods employed to determine risk accuracy of high-risk and low-risk loans, there are several outcomes of varying accuracy. The Easy Ensemble Ada Boost Classifier resulted in the highest accuracy at 0.94, while the other methods ranged from 0.4 to 0.91 in accuracy. Though we see that the Easy Ensemble Ada Boost Classifier was the best method, one could argue that 0.94 is not high in enough in terms of accuracy to recommend. Another potential model that may yield a result in 0.98 or higher would be preferrable in order to be recommended as a machine learning model.
