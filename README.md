# Credit_Risk_Analysis
# Purpose 
To use different techniques to train and evaluate models based on a credit card dataset with unbalanced classes.  We will be assessing credit risk using models that will oversample the data, under sample the data, or use a combination of the two to sample the data.  Then we will use two machine learning models that reduced bias and predict credit risk. 

# Results

**RandomOversampler**

Accuracy Score:

0.8325468421491353

Precision and Recall 
![RandomOverSampler](https://user-images.githubusercontent.com/92542382/155917817-b7312784-c156-40e2-b73e-4c8e30968866.PNG)

**SMOTE Oversampling**

Accuracy Score:

0.8440938486973113

Precision and Recall 

![SMOTE](https://user-images.githubusercontent.com/92542382/155918130-20048010-1b24-4105-841e-60e10a144e63.PNG)

**Undersampling (ClusterCentroids)**

Accuracy Score:

0.8203882595930314

Precision and Recall 

![Undersampling](https://user-images.githubusercontent.com/92542382/155918225-28d38dd2-a371-4b9a-abce-bb5f0e270a6c.PNG)

**Combination (Over and Under) Sampling (SMOTEENN)**

Accuracy Score:

0.844016280135965

Precision and Recall 

![Combo](https://user-images.githubusercontent.com/92542382/155918320-08fac51a-076f-4b01-8bff-fa21906fa743.PNG)

**Balance Random Forest Classifier**

Accuracy Score:

0.784

Precision and Recall 

![randomforest](https://user-images.githubusercontent.com/92542382/155918438-f3536038-2767-4db9-a2d9-c2e5b0b80c56.PNG)

**Easy Ensemble AdaBoost Classifier**

Accuracy Score:

0.931601605553446

Precision and Recall 

![easyensemble](https://user-images.githubusercontent.com/92542382/155918536-e78cf897-5fb9-4449-8d10-10fcb6c2764c.PNG)

# Summary 

As you can see above the,  precision and F1 scores of the RandomOverSampler,  SMOTE, Undersampler (ClusterCentroid),  Combination (SMOTEENN), and Balance Random Forest Classifier methods are much too low to warrant their use as models for high risk credit.   However, they would be great models to predict low risk credit.

The EasyEnsemble was the best model in predicting high risk credit with an f1 score of .16 and recall score of .92.  This is despite a precision score of only .09. 

In relation to the scores of the other models, I would recommend using the EasyEnsemble method.

