**Athlete Injury Risk Prediction Model**

**Project Overview**

This project applies predictive modeling to identify athletes at elevated injury risk using performance and training-related metrics. The goal is to support data-driven injury prevention and workload management decisions.

**Business Problem**

Injuries result in missed practice time, reduced performance, and increased rehabilitation demands. This project aims to estimate injury probability using measurable training and fatigue indicators to assist coaching and sports medicine staff in early intervention.

**Dataset**

200 collegiate athletes

17 performance and workload-related variables

7% injury rate (class imbalance)

**Methodology**

Data preprocessing and one-hot encoding

Stratified train-test split to preserve injury ratio

Logistic Regression with class_weight='balanced'

Model comparison with and without ACL_Risk_Score to assess potential data leakage

Evaluation metrics emphasized recall due to injury rarity

**Key Findings**

Higher fatigue and training intensity were associated with increased injury probability.

Load balance score demonstrated strong protective association.

Model achieved 100% recall (test set) when including ACL_Risk_Score.

Removal of ACL_Risk_Score reduced recall significantly, highlighting predictive dependence and potential leakage concerns.

**Limitations**

Small dataset with limited injury cases

Metrics sensitive to small test sample size

External validation required before deployment

**Tools Used**

Python

Pandas

Scikit-learn

Matplotlib / Seaborn
