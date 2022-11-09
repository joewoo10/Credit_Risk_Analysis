# Credit_Risk_Analysis

## Overview of the Loan Prediction Risk Analysis

### Purpose

A hypothetical peer to peer lending services company wants to use machine learning to predict credit risk. They need help building and evaluating several ML models, oversampling and undersampling the data, and assessing the performance of the models to see how well they predict data. It's management's belief that this will provide a quicker and more reliable loan experience, and lead to a more accurate identification of good candidates for loans.

## Results

### Outputs from the Six Learning Models

•	The naive random oversampling algorithm resulted in a balanced accuracy score of 0.637. The precision score was 1.0 for predicting low risk, but very low for predicting high risk: 0.01. The recall scores were 0.62 and 0.65 for high and low risk, respectively.

![image](https://user-images.githubusercontent.com/109227896/200950107-186c50ae-f1d8-42ce-ad71-c2962dd9ef80.png)

•	The SMOTE algorithm resulted in a balanced accuracy score of 0.63. The precision for predicting high and low risk was identical to the naive random oversampling algorithm. The recall scores were 0.62 and 0.64 for high and low risk, respectively.

![image](https://user-images.githubusercontent.com/109227896/200950186-00671059-96a6-406c-89bb-0af94c95171d.png)

•	The Cluster Centroids algorithm resulted in a balanced accuracy score of 0.63. The precision for predicting high and low risk was the same as the two previous algorithms. The recall scores were 0.59 and 0.43 for high and low risk, respectively.

![image](https://user-images.githubusercontent.com/109227896/200950245-d6416fed-4faa-434f-a93d-977f9454ad76.png)

•	The SMOTEENN algorithm resulted in a balanced accuracy score of 0.51. The precision for predicting high and low risk was the same as all the previous algorithms. The recall scores were 0.70 and 0.57 for high and low risk, respectively.

![image](https://user-images.githubusercontent.com/109227896/200950291-4309e729-dda3-4869-b64c-3c5a0315dbdc.png)

•	The Balanced Random Forest Classifier resulted in a resulted in a balanced accuracy score of 0.789. The precision score was 1.0 for predicting low risk, but very low for predicting high risk: 0.03. The recall scores were 0.70 and 0.87 for high and low risk, respectively.

![image](https://user-images.githubusercontent.com/109227896/200950337-edeffcbc-0a65-491c-bca8-be6fbed83253.png)

•	The Easy Ensemble Classifier resulted in a balanced accuracy score of 0.93. The precision score was 1.0 for predicting low risk, but very low for predicting high risk: 0.09. The recall scores were 0.92 and 0.94 for high and low risk, respectively.

![image](https://user-images.githubusercontent.com/109227896/200950387-469e23e7-d9fa-45ad-a947-172503ab9e8f.png)

## Summary

Resampling the training data with SMOTEEN yielded the lowest balanced accuracy score of 0.51. The precision scores for predicting high risk were low for all six models. The Easy Ensemble Classifier offered the highest recall scores of 0.92 and 0.94 for high and low risk, respectively. I would recommend using the Easy Ensemble Classifier because it easily had the highest balanced accuracy score of 0.93, although the company should be aware of the implications of the precision scores. The precision score of 0.09 means that a high-risk classification is unreliable.
