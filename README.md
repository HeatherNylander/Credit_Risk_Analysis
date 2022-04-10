# Credit Risk Analysis

## Overview
#### Purpose of Analysis
To use the credit card credit dataset from LendingClub, a peer-to-peer lending services company, to oversample the data using the RandomOverSampler and SMOTE algorithms, and undersample the data using the ClusterCentroids algorithm. Then, use a combinatorial approach of over- and undersampling using the SMOTEENN algorithm. Next, to compare two new machine learning models that reduce bias, BalancedRandomForestClassifier and EasyEnsembleClassifier, to predict credit risk. Once done, an evaluation of the performance of these models and a written recommendation on whether they should be used to predict credit risk will be done.

## Results

#### Results of All 6 Machine Learning Models
| Machine Learning Model <img width=1000/>  | Results <img width=1000/> |
| ------------- | ------------- |
| **Naive Random Oversampling** <br />  ![1](https://github.com/HeatherNylander/Credit_Risk_Analysis/blob/main/images/1.png) | • Accuracy Score: 64.7% <br /> • Precision High Risk: 1% <br /> • Precision Low Risk: 100% <br /> • Recall High Risk: 69% <br /> • Recall Low Risk: 60% |
| **SMOTE Oversampling** <br />  ![2](https://github.com/HeatherNylander/Credit_Risk_Analysis/blob/main/images/2.png)| • Accuracy Score: 66.2% <br /> • Precision High Risk: 1% <br /> • Precision Low Risk: 100% <br /> • Recall High Risk: 63% <br /> • Recall Low Risk: 69% |
| **ClusterCentroids Model: Undersampling** <br />  ![3](https://github.com/HeatherNylander/Credit_Risk_Analysis/blob/main/images/3.png)| • Accuracy Score: 54.5% <br /> • Precision High Risk: 1% <br /> • Precision Low Risk: 100% <br /> • Recall High Risk: 69% <br /> • Recall Low Risk: 40% |
| **SMOTEENN Model: Combination Sampling** <br />  ![4](https://github.com/HeatherNylander/Credit_Risk_Analysis/blob/main/images/4.png) | • Accuracy Score: 67.8% <br /> • Precision High Risk: 1% <br /> • Precision Low Risk: 100% <br /> • Recall High Risk: 78% <br /> • Recall Low Risk: 57% |
| **Balanced Random Forest Classifier Model** <br />  ![5](https://github.com/HeatherNylander/Credit_Risk_Analysis/blob/main/images/5.png)| • Accuracy Score: 78.8% <br /> • Precision High Risk: 4% <br /> • Precision Low Risk: 100% <br /> • Recall High Risk: 67% <br /> • Recall Low Risk: 91% |
| **Easy Ensemble AdaBoost Classifier Model** <br /> ![6](https://github.com/HeatherNylander/Credit_Risk_Analysis/blob/main/images/6.png)| • Accuracy Score: 92.5% <br /> • Precision High Risk: 7% <br /> • Precision Low Risk: 100% <br /> • Recall High Risk: 91% <br /> • Recall Low Risk: 94% |


## Summary 
#### Summary of Results
- The EasyEnsembleClassifier model had the higest accuracy score by far with 92.5%. 
- The low risk precision was 100% for all models.
- The high risk precision was very low for all models, ranging from 1% to 7%.

#### Recommendation
- The most accurate model is the EasyEnsembleClassifier model.
- However, The high risk precision was only 7%.
- It is important to note that the original dataset was improperly balanced with far more low risk applications than high risk.
- This model should be run through again with a more balanced dataset.

