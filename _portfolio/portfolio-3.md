---
title: "Portfolio 3: End-to-End Credit Risk Modelling & Portfolio Risk Analytics (UK)"
excerpt: "An end-to-end credit risk modelling project using a large-scale synthetic UK lending dataset to estimate Probability of Default (PD) and quantify portfolio risk through LGD, EAD, and Expected Loss (EL) under stressed macroeconomic conditions. The framework combines interpretable Logistic Regression with advanced machine learning models, enhanced by LIME for local explainability, to support risk-based pricing, optimise decision thresholds, and enable data-driven, Basel II/III-aligned credit decision-making. <br/><img src='/images/calibration curve.png'>" # Preview image
collection: portfolio
---

📎For more details, click [here](https://github.com/Danny-NG-9999/Academic-and-Personal-Projects/tree/main/Economic/Credit%20Risk%20Modeling)


## 🎯 Objective
Built an end-to-end credit risk modelling framework for a UK private bank to predict Probability of Default (PD) and quantify portfolio risk via LGD, EAD, and Expected Loss (EL) under adverse macroeconomic conditions. The project aims to support risk-based pricing, capital allocation, and regulatory-aligned decision-making under Basel II/III principles.

## ⚙️ Tasks
- Data Preprocessing & Cleaning: Handled missing values, treated outliers, and standardised numerical features to ensure data quality and model stability.
- Feature Engineering (WoE/IV): Transformed variables using Weight of Evidence (WoE) and selected features based on Information Value (IV) to enhance predictive power and maintain interpretability.
- Data Splitting & Validation: Implemented a train/test/holdout framework to ensure robust model evaluation and prevent data leakage.
- Model Development (Scorecard & Benchmarking): Built an interpretable Logistic Regression scorecard model and benchmarked performance against ensemble methods (e.g., Random Forest, XGBoost).
- Class Imbalance Handling: Applied resampling techniques (ADASYN, SMOTE variants) to improve detection of rare default events.
- Threshold Optimisation: Tuned classification thresholds using ROC analysis and Youden’s Index to balance sensitivity and specificity, prioritising recall.
- Model Evaluation & Validation: Assessed performance using ROC-AUC, Gini coefficient, KS statistic, CAP curve, and confusion matrix metrics to evaluate discrimination and classification effectiveness.
- Risk Quantification (LGD, EAD, EL): Implemented LGD and EAD estimation and calculated Expected Loss (EL = PD × LGD × EAD) to translate model outputs into monetary risk measures.

## 💡 Results
- Model performance: Logistic Regression achieved ROC-AUC = 0.9524, Gini = 0.9048, and KS = 0.7703, with 92.73% recall, effectively capturing the majority of defaulters.
- Risk drivers: Loan-to-value, interest rate and regularity of income inflows (IV > 0.5) were identified as the primary predictors, outperforming traditional variables such as income level and employment length.
- Business impact: Reduced missed defaults to 554 out of 7,617, significantly limiting loss exposure. CAP analysis showed that ~90% of defaulters were captured within the top 20% of the highest-risk segment, enabling more targeted and efficient underwriting.
- Financial integration: The Expected Loss (EL) framework translated model outputs into monetary terms (e.g., rejecting a small business loan with EL = £39.7k versus approving a home improvement loan with EL = £42), supporting automated credit decision-making and portfolio risk optimisation.