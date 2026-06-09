---
title: "Portfolio 3: Basel-Aligned Multi-Stage Credit Risk Modeling Framework: Development and Application (White-Box model)"
excerpt: "A Basel-aligned multi-stage credit risk modeling framework built on ~250,000 Lending Club consumer loans, estimating Probability of Default (PD), Loss Given Default (LGD), and Exposure at Default (EAD) using transparent white-box models. The framework integrates class-weighted logistic regression, a two-stage LGD hurdle model, and Credit Conversion Factor (CCF)-based EAD estimation to generate Expected Loss (EL) forecasts. Independently validated on a 50,000-loan holdout sample, supporting risk-based pricing, stress testing, capital planning, and portfolio credit risk management. <br/><img src='/images/Lending's Club EDA.png'>" # Preview image
collection: portfolio
---

📎For more details, click [here](https://github.com/Danny-NG-9999/Academic-and-Personal-Projects/tree/main/Economic/Multi-Stage%20Credit%20Risk%20Modeling)

## 🎯 Objective
Developed a comprehensive, white-box, Basel-compliant multi-stage credit risk modeling framework to estimate Probability of Default (PD), Loss Given Default (LGD), Exposure at Default (EAD), and Expected Loss (EL) using real-world Lending Club data. The project aims to provide transparent, interpretable, and regulator-friendly risk quantification to support credit underwriting, portfolio monitoring, risk-based pricing, and capital planning.

## ⚙️ Tasks
- **Data Preparation & Feature Engineering**
    - Processed over 250,000 loan records from a raw dataset of 152 variables, addressing missing values, outliers, and inconsistent entries through systematic and robust data cleaning to establish a stable and audit‑ready modeling baseline
    - Engineered and selected 34 high‑predictive features using a rigorous multi‑step process:
        - Multicollinearity assessment: Applied Variance Inflation Factor (VIF) and Condition Index (CI) to detect and remove redundant variables, ensuring model stability and interpretability.
        - Predictive power assessment: Used Weight of Evidence (WoE) transformation and Information Value (IV) to quantify variable predictive strength and retain features with meaningful discriminatory power relatives to default and recovery outcomes.
    - This approach ensured a parsimonious, interpretable feature set that balances predictive performance with model transparency, while minimizing data leakage, reducing overfitting risk, and aligning with best practices for regulatory credit risk modeling and scorecard development.

- **Probability of Default (PD) Modeling**
    - Developed a class-weighted Logistic Regression scorecard model.
    - Applied Youden's Index for threshold optimisation.
    - Evaluated using ROC-AUC, Gini, KS Statistic, Recall, Precision and CAP curve

Handling class imbalance: Built a class‑weighted Logistic Regression scorecard that directly accounts for the rare nature of defaults, avoiding artificial resampling and preserving the natural default rate for better calibration.

Threshold optimisation: Applied Youden’s Index to select an optimal classification threshold, deliberately prioritising recall (72%) over precision to minimise the costly error of missing actual defaults – a strategic choice for credit risk.

Comprehensive evaluation: Assessed model performance using a full suite of metrics – ROC‑AUC and Gini for ranking ability, KS for separation power, recall and precision for classification trade‑offs, and Brier score for probability calibration – ensuring the model is both discriminative and well‑calibrated.



    Built a class‑weighted Logistic Regression scorecard model to directly handle severe class imbalance (rare defaults).

Optimised the classification threshold using Youden’s Index, balancing sensitivity and specificity with a deliberate preference for high recall (catching defaults).

Evaluated discrimination and calibration via ROC‑AUC, Gini coefficient, KS statistic, recall, precision, and Brier score – ensuring both ranking ability and probability accuracy.

Loss Given Default (LGD) Modeling
Implemented a two-stage hurdle framework:
Stage 1: Logistic Regression predicting recovery occurrence.
Stage 2: Linear Regression (OLS) estimating recovery magnitude.
Exposure at Default (EAD) Modeling
Developed a Credit Conversion Factor (CCF) based Linear Regression model to estimate exposure at the point of default.
Model Validation
Conducted independent out-of-sample validation using a 50,000-loan holdout dataset to assess robustness and generalisation performance.

## 💡 Results





## ⚙️ Tasks
- **Data Preparation:** Cleaned and processed ~250k Lending Club loans (2017–2018) with 152 raw features; reduced to 34 predictive variables via VIF, Condition Index, WoE, and IV analysis.
- **PD Modelling:** Built a class‑weighted logistic regression model with Youden’s index threshold optimisation to prioritise default detection (recall).
- **LGD Modelling:** Developed a two‑stage framework – Stage 1 (logistic regression) predicts recovery likelihood; Stage 2 (OLS) estimates recovery magnitude conditional on recovery.
- **EAD Modelling:** Estimated exposure at default using a linear regression based on Credit Conversion Factor (CCF) approach.
- **Validation:** Independently validated all models on a 50k‑loan holdout set (same period) to assess generalisation and overfitting.
- **Risk Integration:** Combined PD × LGD × EAD into an Expected Loss (EL) metric for portfolio‑level loss forecasting.

## 💡 Results
- **PD Model:** ROC‑AUC = 0.77, Gini = 0.53, KS = 0.40, Recall = 72% – strong default detection and ranking ability for retail portfolios.
- **LGD Stage 1:** ROC‑AUC = 0.72, Recall = 84% – effectively identifies recoverable default accounts.
- **LGD Stage 2:** MAE = 0.03, RMSE = 0.05 – low prediction errors, though R² = 0.02 reflects inherent noise in recovery outcomes (legal actions, collection strategies, etc.).
- **EAD Model:** R² = 0.35, MAE = 0.08 – solid predictive power for exposure, more predictable than LGD.
- **Holdout Validation:** Minimal performance decay (ROC‑AUC Δ = 0.0039, MAE Δ ≤ 0.012), confirming robust generalisation and no overfitting.
- **Business Impact:** Framework translates borrower data into monetary loss estimates, enabling automated credit decisions, capital allocation, and stress‑testing – all within a transparent, Basel‑compliant structure.