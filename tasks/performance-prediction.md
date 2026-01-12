---
# Student Prediction Tasks
  
| Task | Dataset | Algo | Metrics | Approach | Best Algo | Ref | Code | 
| -------------- | ---------------- | ------------ | -------------- | ------------------------- | ----------- | ---- | ---- |
| Pass, Fail, Withdraw, and Binary btw each | OULAD (demographics, virtual learning interactions, and weekly assessment scores), 25,793 students, | RF,SVM,KNN | Accuracy, F1 | early and late fusion, 5 cross-validatoin, SMOTE |  RF with early fusion and SMOTE with 81.67% accuracy for multiclass and 97.45% accuracy for binary class| [2025](https://github.com/soklayheng/AIED/blob/main/references/AStudentPerformancePredictionModelUsingMachineLearningModelsinM.pdf)|  |
| Drop vs Success | Real-world online education, 35,000 samples, 49 features, socio-demographic, behavioral and students'comments on online course interaction (sentiment), test with next year data | Finetuned BERT for sentimental, and XGBoost, RF, and LR |Accuracy, Precison, Recall | cross-validation, sentimental analysis integration for prediction, hyper-tunning, SHAP in preprocessing for feature importance | XGBoost + Sentimental (84% Acc) |[2025](https://github.com/soklayheng/AIED/blob/main/references/2507.10421v1.pdf) | |
| Regular vs Non-regular | Indonesian Institute (demographic, activity and achievement data), train-test (75:25), 20 features | Precision, Recall, F1| | SMOTE | LR with 91% accuracy  | [2022](https://github.com/soklayheng/AIED/blob/main/references/Predicting_Computer_Science_Students_Performance_using_Logistic.pdf) |  |
| At risk vs Non-risk | 3 public dataset: HEI, HESP, XAPI; Demographic, Academic, and Behavior, train:test(80:20) | CNN + BIGRU, ANN and LSTM, BILSM, GRU, BIGRU | Accuracy, Precison, Recall, and F1 | hybrid DNN, SMOTE, hyper-tune | CNN + BIGRU with accuracy of 97.48%,90.90%, and 95.97% across the three datasets | [2025](https://github.com/soklayheng/AIED/blob/main/references/mca-30-00059.pdf)|  |

