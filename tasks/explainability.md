<!---
# Student Dropout Prediction

## Dataset
- **ASSISTments**: description…

## Metrics
- AUC (higher better)
- Accuracy
-->

---
# Explainability and Interpretability
  
| Task | Dataset | Algo | Metrics | Approach | Best Algo | Ref | Code | 
| -------------- | ---------------- | ------------ | -------------- | ----------------------------------- | ----------- | ---- | ---- |
| Drop vs Success, Fairness | K12 Morocon (academic, demographic, and socio-economic features( 4 sensitive features (gender, handicaps, boarding school availability, and financial aid))| Bagging, Adaptive Boosting (AB) with DT, Stacking (DT,LR,NB) as base and LR as meta-learner. Voting(soft and hard using DT, LR, and NB | AUC, class-specific precision & recall and ABROCA and Demographic Parity between each group pair | --- | Stacking and LR with 0.80 AUC | [2025](https://github.com/soklayheng/AIED/blob/main/references/978-3-031-98462-4_46.pdf) | ---- | 
| Score Prediction, Explainability for both local and global levels | Public : CodeWorkout, 772 students, code submission info for different assignments | stacked ensemble model (KNN, SVM, and XGBoost) as the base models and LR as the meta-model, begging, boosting, LR | RMSE and R<sup>2</sup>| K-Fold 10, hyper-tune, SHAP for individual and a global level (feature importance); force plot + summary plot for individual explanation and shap value for global | Stacked ensemble model | [2023](https://github.com/soklayheng/AIED/blob/main/references/2023.EDM-long-papers.7.pdf) | ---- |
| Final exam score prediction, Interpretability for global level | Real-world Chinese Wuhan Univ (Academic Score: exam scores, Engagement, Psychological :motivation, SRL, learning attitudes, Demographic), and Self-directed Learning, 82 students, train:test(80:20)| RF, Back Propagation Neural Network, SVM, XGBoost | MAE and R<sup>2</sup> | SHAP for global only ; Summary Plot + The average SHAP value plot| XGBoost | [2024](https://github.com/soklayheng/AIED/blob/main/references/journal.pone.0309838.pdf)| ---- |
| Pass vs Fail, Explainability for boot local and global level | Public: OULAD (demographics, assessment scores, and behavioral features (e.g. clicks and attempts))| RF, Extra Trees, CatBoost, XGBoost, NB, KNN | accuracy, recall, precision, and F1-Score | SMOTE,K-Fold 10, hyper-tune with randomized search, SHAP for both global and local. summary plots, bar plots, and dependence plots for global. force plots, decision plots, and waterfall plots for local.|Extra Trees with 0.9537 Acc| 
[2024](https://github.com/soklayheng/AIED/blob/main/references/Analyzing_the_Interpretability_of_Machine_Learning_Prediction_on.pdf)| ---- |


