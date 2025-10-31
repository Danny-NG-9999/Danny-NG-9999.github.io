---
title: "Portfolio 3: King County Housing Market Analysis and Price Prediction: Data-Driven Valuation of Residential Real Estate (USA)"
excerpt: "A comprehensive data analytics and machine learning project focused on residential property valuation in King County, Washington. Leveraging Python and statistical modeling, the study explores key market drivers, price dynamics, and renovation ROI to deliver actionable insights for investors, policymakers, and real estate professionals. <br/><img src='/images/Renovation Premium by City (%) with P-values.png'>"
collection: portfolio
---

📎For more details, click [here](https://github.com/Danny-NG-9999/Academic-and-Personal-Projects/tree/main/Data%20Analysis/House%20Price%20Prediction)


## 🎯 Objective

The project aimed to develop a robust, data-driven framework for understanding and predicting residential housing prices in King County, Washington (2014). By integrating machine learning modeling with market analytics, it sought to identify key value drivers, quantify geographic price disparities, and generate actionable insights for investors, policymakers, and real estate professionals.

## ⚙️ Tasks
- Data Preparation: Cleaned and transformed ~4,600 raw property records into a refined dataset of 4,401 entries through outlier removal, feature engineering, and variable standardization.
Exploratory Analysis: Investigated relationships among property size, amenities, renovation history, and location, highlighting the structural and geographic determinants of price variation.
Model Development: Trained and evaluated multiple regression models (Linear, Lasso, Decision Tree) using an 80/20 train-test split; assessed using R², MAE, RMSE, and cross-validation for performance stability.
Insight Derivation: Analyzed renovation ROI, market segmentation, and city-level pricing trends to uncover region-specific investment opportunities and constraints.

## 💡 Results
- Model Performance: Achieved an R² of 0.76 on test data and MAE of ~$105K, explaining ~76% of price variance with strong generalization across mid-market properties.
- Key Price Drivers: sqft_living (≈0.70 correlation) emerged as the strongest predictor, followed by bathrooms, city, bedrooms, and view. Condition and waterfront factors showed minimal influence.
- Market Insights:
    - Premium zones (cities such as Medina, Clyde Hill, Mercer Island, etc.) priced 2–3× above county average.
    - Mid-tier areas (cities around $400K–$700K) formed the market’s stable core.
    - Affordable segments (cities below $400K) offered entry-level options with limited growth.

- Renovation ROI: Positive returns (+10–13%) in affluent cities; negative returns (–20% to –28%) in saturated markets like SeaTac and Tukwila.
- Strategic Takeaway: Housing prices are driven by living space, location, and selective renovation strategy — emphasizing the need for location-specific investment and pricing decisions.