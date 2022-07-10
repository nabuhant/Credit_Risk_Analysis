# Credit_Risk_Analysis
 Module17_Supervised Machine Learning

# Overview
Using the Scikit-learn library to train and test 6 different machine learning models that follow diffrent techniques in the analysis of the provided credit card dataset. This is done to predict the credit risk of the customers.

# Results
## 1. Naive Random Oversampling Model
- Balanced Accuracy Score: 66.2% (moderate performance)
- High-risk Precision & Sensitivity: 0.01 (very low) & 0.72
- Low-risk Precision & Sensitivity: 1.00 (very high) & 0.60  
This model is not very trustworthy at predicting high-risk cases. Although the high-risk sensitivity is moderately high, the precision is very low with an F1 score of 0.02 that demonstrates an imbalance between the metrics above for high-risk.
![image](/Results/1.png)
 
## 2. SMOTE Oversampling Model
- Balanced Accuracy Score: 65.7% (moderate performance)
- High-risk Precision & Sensitivity: 0.01 (very low) & 0.61
- Low-risk Precision & Sensitivity: 1.00 (very high) & 0.70  
Similarly this model is not very trustworthy at predicting high-risk cases as its performance is very similar to the Naive Random model.
![image](/Results/2.png)
 
## 3. ClusterCentroids Undersampling Model
- Balanced Accuracy Score: 54.5% (low to moderate performance)
- High-risk Precision & Sensitivity: 0.01 (very low) & 0.69
- Low-risk Precision & Sensitivity: 1.00 (very high) & 0.40  
Similarly this model is not very trustworthy at predicting low and high-risk cases.
![image](/Results/3.png)
 
## 4. SMOTEENN Over and UnderSampling Model
- Balanced Accuracy Score: 63.9% (low to moderate performance)
- High-risk Precision & Sensitivity: 0.01 (very low) & 0.69
- Low-risk Precision & Sensitivity: 1.00 (very high) & 0.59  
This model performed better than the previous models, yet it is still not very trustworthy at predicting high-risk cases.
![image](/Results/4.png)
 
## 5. Balanced Random Forest Classifier Model
- Balanced Accuracy Score: 78.9% (low to moderate performance)
- High-risk Precision & Sensitivity: 0.03 (very low) & 0.70
- Low-risk Precision & Sensitivity: 1.00 (very high) & 0.87  
This model's accuracy & precision performed better than all previous resampling models, and had an increased F1 score for both high-risk and low-risk cases.  
![image](/Results/5.png)
 
## 6. Easy Ensemble Classifier Model
- Balanced Accuracy Score: 93.2% (low to moderate performance)
- High-risk Precision & Sensitivity: 0.09 (very low) & 0.92
- Low-risk Precision & Sensitivity: 1.00 (very high) & 0.94  
This model's accuracy, precision, & sensitivuty performed better than all previous models, and had an increased F1 score for both high-risk and low-risk cases.
This model is the best in carrying out the prediction required for this project.
![image](/Results/6.png)
 
# Summary
## Results
Overall the resmpling models (1-4) performed relatively the same with accuracies between mid-50s to mid-60s. The precision for all 4 models were the same for the low-risk and high-risk cases. The models had varied sensitivities but consistently low F1 scores for the high-risk prediction, therefore the models could not be determined to have a good fit in predicting. The ensemble models had higher accuracies, precision, and sensitivities/recalls with increased F1 scores.
## Recommendation
The model that is recommended for use is the Easy Ensemble Classifier model, with the highest accuracy of 93.2% and high-risk precision of 0.09 (sensitivity 0.92 and highest F1 score of 0.16). It also performs very well in predicting low-risk cases with precision of 1.00 (sensitivity 0.94 and high F1 score of 0.97).
