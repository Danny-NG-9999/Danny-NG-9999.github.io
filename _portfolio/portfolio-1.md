---
title: "Portfolio 3: Basel-Aligned Multi-Stage Credit Risk Modeling Framework: Development and Application (White-Box model)"
excerpt: "A Basel-aligned multi-stage credit risk modeling framework built on ~250,000 Lending Club consumer loans, estimating Probability of Default (PD), Loss Given Default (LGD), and Exposure at Default (EAD) using transparent white-box models. The framework integrates class-weighted logistic regression, a two-stage LGD hurdle model, and Credit Conversion Factor (CCF)-based EAD estimation to generate Expected Loss (EL) forecasts. Independently validated on a 50,000-loan holdout sample, supporting risk-based pricing, stress testing, capital planning, and portfolio credit risk management. <br/><img src='/images/lending_overview.png'>" # Preview image
collection: portfolio
---


📎For more details, click [here](https://github.com/Danny-NG-9999/Academic-and-Personal-Projects/tree/main/Economic/Credit%20Risk%20Modeling)


## 🎯 Objective
Developed a credit risk model to support lending decisions and reduce default-related losses for a UK private bank to predict Probability of Default (PD) and quantify portfolio risk via LGD, EAD, and Expected Loss (EL) under adverse macroeconomic conditions. The project aims to support risk-based pricing, capital allocation, and regulatory-aligned decision-making under Basel II/III principles.

## ⚙️ Tasks
- **Data Preprocessing & Cleaning:** Handled missing values, treated outliers, and standardised numerical features to ensure data quality and model stability.
- **Feature Engineering (WoE/IV):** Transformed variables using Weight of Evidence (WoE) and selected features based on Information Value (IV) to enhance predictive power and maintain interpretability.
- **Data Splitting & Validation:** Implemented a train/test/holdout framework to ensure robust model evaluation and prevent data leakage.
- **Model Development (Scorecard & Benchmarking):** Built an interpretable Logistic Regression scorecard model and benchmarked performance against ensemble methods (e.g., Random Forest, XGBoost).
- **Class Imbalance Handling:** Applied resampling techniques (ADASYN, SMOTE variants) to improve detection of rare default events.
- **Threshold Optimisation:** Tuned classification thresholds using ROC analysis and Youden’s Index to balance sensitivity and specificity, prioritising recall.
- **Model Evaluation & Validation:** Assessed performance using ROC-AUC, Gini coefficient, KS statistic, CAP curve, and confusion matrix metrics to evaluate discrimination and classification effectiveness.
- **Risk Quantification (LGD, EAD, EL):** Implemented LGD and EAD estimation and calculated Expected Loss (EL = PD × LGD × EAD) to translate model outputs into monetary risk measures.

## 💡 Results
- **Model performance:** Logistic Regression achieved ROC-AUC = 0.9524, Gini = 0.9048, and KS = 0.7703, with 92.73% recall, effectively capturing the majority of defaulters.
- **Risk drivers:** Loan-to-value, interest rate and regularity of income inflows (IV > 0.5) were identified as the primary predictors, outperforming traditional variables such as income level and employment length.
- **Business impact:** Reduced missed defaults to 554 out of 7,617, significantly limiting loss exposure. CAP analysis showed that ~90% of defaulters were captured within the top 20% of the highest-risk segment, enabling more targeted and efficient underwriting.
- **Financial integration:** The Expected Loss (EL) framework translated model outputs into monetary terms (e.g., rejecting a small business loan with EL = £39.7k versus approving a home improvement loan with EL = £42), supporting automated credit decision-making and portfolio risk optimisation.