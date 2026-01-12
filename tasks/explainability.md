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

<div class="table-wrap">
  
| Task | Dataset | Algo | Metrics | Approach | Best Algo | Ref | Code | 
| -------------- | ---------------- | ------------ | -------------- | ----------------------------------- | ----------- | ---- | ---- |
| Drop vs Success, Fairness | K12 Morocon (academic, demographic, and socio-economic features( 4 sensitive features (gender, handicaps, boarding school availability, and financial aid)), 2015/2016 to 2019/2020 school years as the training set and 2020/2021 school year as the test set | Bagging, Adaptive Boosting (AB) with DT, Stacking (DT,LR,NB) as base and LR as meta-learner. Voting(soft and hard using DT, LR, and NB | AUC, class-specific precision & recall and ABROCA and Demographic Parity between each group pair | Different ensembled methods | Stacking and LR with 0.80 AUC, different results of ABROCA and DP from one model to another according to different attribute | [2025](https://github.com/soklayheng/AIED/blob/mainreferences/978-3-031-98462-4_46.pdf) | | 
| Score Prediction, Explainability for both local and global levels | Public : CodeWorkout, 772 students, code submission info for different assignments only, 7 features | stacked ensemble model (KNN, SVM, and XGBoost) as the base models and LR as the meta-model, begging, boosting,KNN, SVM, XGBoost, LR | RMSE and R<sup>2</sup>| K-Fold 10, hyper-tune, SHAP for individual and a global level (feature importance); force plot + bar plot for individual explanation and summary plot for global | Stacked ensemble model with 0.151 RMSE and 0.55 R<sup>2</sup> | [2023](https://github.com/soklayheng/AIED/blob/main/references/2023.EDM-long-papers.7.pdf) | |
| Final exam score prediction, Interpretability for global level | Real-world Chinese Wuhan Univ (Academic Score: exam scores, Engagement, Psychological :(motivation, SRL, learning attitudes), Demographic, and Self-directed Learning), 87 students, train:test(80:20), 9 features| RF, Back Propagation Neural Network, SVM, XGBoost | MAE and R<sup>2</sup> | SHAP for global only ; Bar Plot + Summary Plot| XGBoost with MAE of 6 and R<sup>2</sup> of 0.82 | [2024](https://github.com/soklayheng/AIED/blob/main/references/journal.pone.0309838.pdf)| |
| Pass vs Fail, Explainability for both local and global levels | Public: OULAD (demographics, assessment scores, and behavioral features (e.g. clicks and attempts)), 4,434 student recordes, 17 features| RF, Extra Trees, CatBoost, XGBoost, NB, KNN | accuracy, recall, precision, and F1-Score | SMOTE,K-Fold 10, hyper-tune with randomized search, SHAP for both global and local. summary plots, bar plots, and dependence plots for global. force plots, decision plots, and waterfall plots for local.|Extra Trees with 0.9537 Accuracy| [2024](https://github.com/soklayheng/AIED/blob/main/references/Analyzing_the_Interpretability_of_Machine_Learning_Prediction_on.pdf)| |
| Drop vs Success but also project probability with bias correction, Explainability for both local and global levels, user study for explainablity evaluation| Real-world: Budapest University of Technology (pre-enrollment achievement measures + demographic + previous record (highschool GPA)),8,508 students,2013&2016 as train and 2017 as test | CATBOOST, LR | AUC | Project probability of dropout by making corrections using Platt’s calibration and the isotonic regression method, use different XML such as permutation importance (PI) and catboost built-in feature importance: to estimate feature importance for global, two-dimensional partial dependence plot (PDP):to study relationship between feature for global, LIME for local, and SHAP for global and local and compare it with LIME , user experience research | CATBOOST with 0,77 AUC and 0,84 precision| [2023](https://github.com/soklayheng/AIED/blob/main/references/s40593-023-00331-8.pdf) | |

</div>


