# Insurance-Churn-Prediction-Using-PyCaret
MachineHack Competition

In this hackathon, the project was all about 'insurance churn prediction'. The training dataset provided is highly imbalanced: only ~11% churn rate. Another one bottleneck in this project was that we had 16 anonymized features. Thus, feature engineering by employing domain knowledge is also not possible. In my second attempt (not presented in this ipynb) new fatures were generated using automated feature engineering (by feature tools) and it landed up with total features of 256. After PCA, several models were attempted, even with oversampling. All the traing results were fantastic but the models perfomed relatively poor with the unseen data. After getting stucked, thought of learning something new and tried PyCaret for the first time. The library looks super cool and works amazingly well. Here I have not done any oversampling but could identify four best performers, namely, lightgbm, catboost, gbc and xgboost. As per the F1 score (evaluation criteria for this hackathon), lightgbm was best with a F1 score of 0.56. As expected, stacking improved the performance and pushed up the F1 score to 0.58.
