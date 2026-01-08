---
# Student Prediction Tasks
  
| Task | Dataset | Algo | Metrics | Approach | Best Algo | Ref | Code | 
| ---- | ------- | ---- | ------- | --------- | --- | ---- | ---- |
| Multi-classificaiton: Pass, Fail, Withdraw, and binary | OULAD (demographics, virtual learning interactions, and assessment scores) | RF,SVM,KNN | Accuracy, F1 | early and late fusion, 5 cross-validatoin, SMOTE |  RF with early fusion and SMOTE | [2025](https://github.com/soklayheng/AIED/blob/main/references/AStudentPerformancePredictionModelUsingMachineLearningModelsinM.pdf)|  |
| Bi-classification: drop vs success | Real-world online educationm, 35,000 samples, 49 features, socio-demographic, behavioral and comment(sentiment), test with next year data | Finetuned BERT
for sentimental, and XGBoost, RF, and Log Reg |Accuracy, Precison, Recall | cross-validation, sentimental analysis integration for prediction, hyper-tunning, SHAP in preprocessing for feature importance | XGBoost + Sentimental (84% acc)|[2025](https://github.com/soklayheng/AIED/blob/main/references/2507.10421v1.pdf) | |
