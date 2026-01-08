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
| -------------- | ---------------- | ------------ | -------------- | ------------------------- | ----------- | ---- | ---- |
| Drop vs Success, Fairness | k12 Morocon (academic, demographic, and socio-economic
features( 4 sensitive features (gender, handicaps, boarding school availability, and financial aid))| Bagging, Adaptive Boosting (AB) with DT, Stacking (DT,LR,NB) as base and LR as meta-learner. Voting(soft and hard using DT, LR, and NB | AUC, class-specific precision & recall and ABROCA and Demographic Parity between each group pair | --- | Stacking and LR with 0.80 AUC | [2025] (https://github.com/soklayheng/AIED/blob/main/references/978-3-031-98462-4_46.pdf) | ---- | 
