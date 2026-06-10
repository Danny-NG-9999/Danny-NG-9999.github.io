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
        - **Multicollinearity assessment:** Applied Variance Inflation Factor (VIF) and Condition Index (CI) to detect and remove redundant variables, ensuring model stability and interpretability.
        - **Predictive power assessment:** Used Weight of Evidence (WoE) transformation and Information Value (IV) to quantify variable predictive strength and retain features with meaningful discriminatory power relatives to default and recovery outcomes.
    - This approach ensured a parsimonious, interpretable feature set that balances predictive performance with model transparency, while minimizing data leakage, reducing overfitting risk, and aligning with best practices for regulatory credit risk modeling and scorecard development.

- **Probability of Default (PD) Modeling**
    - **Handling class imbalance:** Developed a class-weighted Logistic Regression scorecard to address the inherently low default rate within consumer lending portfolios. This approach preserves the natural class distribution while improving the model's ability to identify high-risk borrowers without relying on synthetic resampling techniques.
    - **Risk-Based Threshold Optimization:** Optimized the classification threshold using Youden's Index, balancing sensitivity and specificity while intentionally prioritizing default detection (72% Recall). This reflects a practical credit-risk strategy where failing to identify a future defaulter is significantly more costly than generating additional false-positive alerts.
    - **Scorecard Development & Interpretability:** Leveraged a transparent white-box modeling framework to produce interpretable borrower risk scores, enabling clear explanation of lending decisions and alignment with regulatory expectations under Basel IRB principles.
    - **Comprehensive Model Validation:** Evaluated discriminatory power, ranking performance, classification effectiveness, and probability calibration using a robust suite of metrics including ROC-AUC (0.77), Gini (0.53) and KS Statistic (0.40). This ensured the model not only differentiates effectively between good and bad borrowers but also produces reliable default probability estimates suitable for downstream LGD, EAD, and Expected Loss calculations.

- **Loss Given Default (LGD) Modeling**
    - Developed a two-stage LGD framework to reflect the real-world recovery process following borrower default. Rather than treating all recovery outcomes identically, the model separates the decision of whether any recovery occurs from the estimation of how much is ultimately recovered.
        - **Stage 1 – Recovery Classification:** A class-weighted Logistic Regression model predicts whether a defaulted loan will generate any recovery proceeds, distinguishing recoverable accounts from complete write-offs.
        - **Stage 2 – Recovery Rate Estimation:** For loans predicted to have recoveries, an Ordinary Least Squares (OLS) regression model estimates the magnitude of the recovery rate.
    - **Business Value:** Recovery outcomes are typically characterized by a large proportion of zero recoveries (no recovery) alongside a smaller number of positive recoveries. By modeling these processes separately, the framework better captures the underlying recovery dynamics, improves predictive stability, and provides more transparent estimates for loss forecasting, capital provisioning, and portfolio risk management.

- **Exposure at Default (EAD) Modeling**
    - Developed a Credit Conversion Factor (CCF) based Linear Regression model to estimate borrower exposure at the point of default. Leveraged loan balance, repayment behaviour, and credit utilization characteristics to model expected exposure levels, supporting Basel-compliant EAD estimation and portfolio-level Expected Loss calculations.

- **Model Validation**
    - Performed independent out‑of‑sample validation using a 50,000‑loan holdout dataset that was completely excluded from model development (feature selection, training, and tuning).
    - Assessed the stability and generalization of all three risk components (PD, LGD, EAD) by comparing key performance metrics between the test set and the holdout set.

## 💡 Results
- **PD Model Performance**
    - ROC‑AUC = 0.77, Gini = 0.53 and KS = 0.40 – Demonstrates strong borrower risk discrimination, significantly above random chance and well within industry acceptance for retail credit scoring.
    - Recall = 72%** – Captures nearly three‑quarters of actual default events, enabling early identification of high‑risk accounts despite severe class imbalance.

- **LGD Model Performance**
    - **Recovery Classification (Stage 1):** ROC‑AUC = 0.72, Recall = 84% – Effectively flags defaulted accounts that will yield any recovery, minimising missed recovery opportunities.
    - **Recovery Rate Estimation (Stage 2):** MAE = 0.03, RMSE = 0.05 – Low prediction errors support reliable estimates of post-default recovery outcomes for portfolio-level loss forecasting.

- **EAD Model Performance**
    - R² = 0.35, MAE = 0.08 – Explains 35% of exposure variability with an average prediction error of 8 percentage points, representing solid predictive performance for estimating borrower exposure at the point of default.
    - Among the three risk components (PD, LGD, EAD), the EAD model demonstrated the strongest out‑of‑sample consistency and stability. This is expected, as EAD is largely driven by observable factors such as remaining loan balance, payment history, and credit utilisation patterns – making it inherently more predictable than loss severity or default probability.


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