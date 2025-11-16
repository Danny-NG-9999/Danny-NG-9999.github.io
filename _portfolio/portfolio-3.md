---
title: "Portfolio 3: Credit Risk Modelling & Default Prediction for Consumer Loan Risk Assessment (UK)"
excerpt: "An end-to-end credit risk analytics evaluation project using a large-scale synthetic UK lending dataset. The study applies logistic regression and XGBoost to estimate default probability, evaluate threshold trade-offs, quantify misclassification losses, and derive portfolio-level insights for risk-based decisioning. <br/><img src='/images/calibration curve.png'>" # Preview image
collection: portfolio
---

📎For more details, click [here](https://github.com/Danny-NG-9999/Academic-and-Personal-Projects/tree/main/Economic/Credit%20Risk%20Modeling%20and%20Evaluation)


## 🎯 Objective
This project aimed to build and validate a predictive credit risk model capable of estimating the probability of loan default in a UK consumer lending environment. Using a 500,000 record synthetic dataset designed to mirror real-world borrower behaviour, the analysis sought to benchmark modelling techniques, assess calibration and ROC performance, and translate model outputs into actionable insights for credit decisioning, risk appetite setting, and portfolio loss mitigation.

## ⚙️ Tasks
- Data Preparation: Cleaned and transformed ~4,600 raw property records into a refined dataset of 4,401 entries through outlier removal, feature engineering, and variable standardization.
Exploratory Analysis: Investigated relationships among property size, amenities, renovation history, and location, highlighting the structural and geographic determinants of price variation.
Model Development: Trained and evaluated multiple regression models (Linear, Lasso, Decision Tree) using an 80/20 train-test split; assessed using R², MAE, RMSE, and cross-validation for performance stability.
Insight Derivation: Analyzed renovation ROI, market segmentation, and city-level pricing trends to uncover region-specific investment opportunities and constraints.

- Data Preparation: Cleaned, validated, and transformed a large-scale synthetic credit dataset; applied one-hot encoding, missing value imputation, and numeric standardisation to ensure consistent model inputs.
- Exploratory Data Analysis: Examined borrower demographics, income distributions, loan characteristics, and interaction effects (e.g., loan-to-income, interest rate tiers). Identified clear relationships between risk bands, loan size, and default propensity.
- Model Development: Implemented and compared Logistic Regression and XGBoost Classifier, using train–test splits, ROC-AUC analysis, calibration curves, threshold sensitivity tests, and feature importance evaluation.
- Financial Impact Assessment: Estimated the expected loss consequences of false negatives (missed defaults) and benchmarked the economic benefits of model improvements.

## 💡 Results
Model Performance:
- XGBoost: AUC = 0.9347, capturing ~94% of defaulters at low false-positive rates and significantly reducing missed-default losses.
- Logistic Regression: AUC = 0.8574, strong baseline but less effective at identifying high-risk borrowers in non-linear regions of the feature space.

Threshold & Portfolio Insights:
- Lower thresholds increased default recall but raised rejection rates; thresholds around 0.35–0.40 provided optimal trade-offs for risk appetite.

Missed-default analysis:
- LR Estimated Loss: £191.8M
- XGBoost Estimated Loss: £116.0M → £75.8M reduction in unrealised losses using XGBoost.

Calibration Results:
- Logistic Regression: optimistic bias, underestimating probability of default in mid-risk segments.
- XGBoost: slight pessimistic bias, but closer alignment with observed outcomes after validation.

Strategic Takeaway:
- Ensemble methods significantly enhance risk discrimination and materially reduce credit losses. Effective credit scoring requires calibrated PD estimates, threshold optimisation, and attention to borrower-level non-linearities.