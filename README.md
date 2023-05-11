# Credit_Risk_Analysis
Using Resampling Models to Predict Credit Risk / Using the SMOTEENN Algorithm to Predict Credit Risk / Using Ensemble Classifiers to Predict Credit Risk

### Overview of the Analysis
- Evaluate the performance of models, allowing us to create a written recommendation on what someone should be using to predict credit risk. 

### Results
1. Oversample: RandomOverSampler - Accuracy Score : 66%

![image](https://github.com/Angel00Michel/Credit_Risk_Analysis/assets/106771574/125e0b7a-4751-460d-bf66-0e485cee1d0e)

- Precision: 1% for high risk, 100% for low risk. 
- Recall: 72% for high risk, 60% low risk.

2. Oversample: SMOTE - Accuracy Score : 66%

![image](https://github.com/Angel00Michel/Credit_Risk_Analysis/assets/106771574/89949729-5018-48f8-859b-edd65533c0fa)

- Precision : 1% for high risk, 100% for low risk
- Recall: 61% for high risk, 70% low risk

3. Undersample using the ClusterCentroids algorithm - Accuracy Score : 54% 

![image](https://github.com/Angel00Michel/Credit_Risk_Analysis/assets/106771574/623915f1-5782-47c2-8564-4273e387352f)

- Precision : 1% for high risk, 100% for low risk
- Recall: 69% for high risk, 40% low risk

4. Combinatorial approach of over- and undersampling using the SMOTEENN algorithm - Accuracy Score : 68%

![image](https://github.com/Angel00Michel/Credit_Risk_Analysis/assets/106771574/d10a5e79-10f6-4960-a1f6-0628c7fcb056)

- Precision : 1% for high risk, 100% for low risk
- Recall: 78% for high risk, 57% low risk

5. BalancedRandomForestClassifier - Accuracy Score : 68%

![image](https://github.com/Angel00Michel/Credit_Risk_Analysis/assets/106771574/c6c79012-010b-4447-82ac-426ce07b50e0)

- Precision : 95% for high risk, 100% for low risk
- Recall: 36% for high risk, 100% low risk

6. EasyEnsembleClassifier - Accuracy Score : 93%

![image](https://github.com/Angel00Michel/Credit_Risk_Analysis/assets/106771574/8ba25122-1089-4a8b-bb03-476a75b0187f)

- Precision : 9% for high risk, 100% for low risk
- Recall: 92% for high risk, 94% low risk

### Summary
- The 'EasyEnsembleClassifier' is the best; among all the models with a 93% Accuracy Score. Its recall rate (92% for high risk, and 94% for low risk) is VERY good compared to the other models. The other models recall rates are not as accurate or as balanced as the 'EasyEnsembleClassifier'. For example the model, 'BalancedRandomForestClassifier', had a 100% low risk recall rate but the high risk recall rate was only 36%. As for the precision of all the models; gives us 100% for the low risk, however most of them are extremely low in term of precision for the high risk, except for the model: 'BalancedRandomForestClassifier'. The 'EasyEnsembleClassifier' is still the preferred model since its recall rate is substantially higher than the others.

