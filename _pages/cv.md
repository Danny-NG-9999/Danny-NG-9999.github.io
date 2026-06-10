---
layout: archive
title: "CV/Resume"
permalink: /cv/
author_profile: true
redirect_from:
  - /resume
---

{% include base_path %}

📎 Download a PDF version of this resume [here](/files/Resume_2026.pdf)


## EDUCATION
***

### MSc Financial Economics | University of Exeter, United Kingdom | September 2024 – September 2025
*   **Degree classification (GPA):** 2:1 (upper second-class honours) 
*   **Key Modules:** Applied Econometric I (64%), Applied Econometric II (63%), Experimental and Behavioural Economics (83%), Economics of Corporate Finance (70%) and Topics in Financial Economics (60%).

*   **Key Achievement:**
    *   **Exeter Award:** Earned the Exeter Award through active participation in workshops, society initiatives like fertilizing soil with coffee grounds, and community projects, showcasing strong teamwork, leadership, and professional skills that enhanced employability and personal growth.
    *   **Green Consultants Project:** Worked in a 4-person team with a doctoral researcher to align academic modules with the UN SDGs, producing a curriculum-mapping framework that was formally recognised with a £100 award for practical value.
    *   **VOIZ Climate Simulation Challenge:** Ranked Top 15 out of 164 teams from 39 UK universities in VOIZ Academy’s national climate case challenge, demonstrating analytical thinking, and effective teamwork under real-world conditions.


## PROFESSIONAL EXPERIENCE
---
### Supervisor | Rosa Thai, United Kingdom | January 2026 - Present

- **Operations and Process Management:** Directed shift-to-shift food and beverage operations, ensuring adherence to presentation standards, portion control, and service time targets. Managed opening and closing procedures using structured checklists to support smooth shift transitions, minimise errors, and maintain audit-ready conditions, while aligning front- and back-of-house teams to deliver consistent performance.
- **Leadership and Cross-Functional Collaboration:** Led structured shift briefings to align team on roles, targets, and priorities, while mentoring new staff on service standards and portion control. Collaborated across front- and back-of-house during peak periods to resolve bottlenecks, support operations (including drink preparation and order packaging), and maintain efficient service delivery within target time frames.
- **Customer Service and Quality Assurance:** Maintained high standards by verifying food and beverage quality prior to service and managing customer queries, complaints, and discretionary adjustments professionally, particularly during peak periods. Coordinated bookings and seating arrangements based on client needs and group size, contributing to consistently positive feedback and a high-quality service experience.
- **Reporting, Data Analysis & Inventory Control:** Maintained accurate inventory records through end-of-day stock counts, date rotation, and labelling compliance; reconciled daily usage against sales data to support effective stock management, cost control, and informed ordering decisions. Produced end-of-shift reports covering sales, customer volumes, SPH, discounts, and operational issues, providing reliable data to support management decision-making and forecasting.


### Transaction Advisory Analyst | Grant Thornton, Vietnam | November 2022 – July 2024 

- **Financial Due Diligence:** Performed detailed reviews of trial balances, general ledgers, and supporting financial statements across 8 M&A transactions (£500k–£8m), identifying and adjusting non-recurring items, misclassified expenses, unusual/suspicious and related-party transactions to establish normalised earnings and support accurate valuation models. Notably uncovered £420k EBITDA adjustment for an FMCG client, which strengthened the buyer’s position in negotiations and drove a more favourable purchase price.
- **Risk and Contract Analysis:** Reviewed customer, supplier, loan, and lease agreements to identify risks such as covenant breaches, termination clauses, contingent liabilities, and FX exposure. Uncovered approximately £500k in unrecorded liabilities (including a £180k take-or-pay penalty, £250k lease termination risk, and £65k restoration obligation) as well as a $1m contingent liability from a cloud services auto-renewal clause. These findings enabled SPA protections and contributed to a 5% reduction in enterprise value. 
- **Revenue, Margin & Concentration Analysis:** Evaluated revenue sustainability, customer concentration, and margin quality through revenue breakdowns, benchmarking, contract mapping and related-party transaction reviews. Identified 15% revenue dependency on a near-term expiring contract and inflated related-party margins (+20%), supporting pricing adjustments and post-deal risk mitigation strategies.
- **Valuation, Reporting and Stakeholder Management:** Supported DCF and comparable company valuation models by preparing operational and capital schedules, and synthesised complex financial and risk findings into client-ready reports and dashboards. Managed VDR and Q&A workflows to ensure timely issue resolution, and contributed sector analysis (renewable energy, regulatory environment) to the Doing Business in Vietnam report.

### Technology Consultant | KPMG, Vietnam | April 2021 – June 2022

- **Risk Testing:** Conducted Tests of Design (ToD) and Tests of Controls (ToC) on IT systems covering access management, change management, and backup processes across multiple engagements. Identified control gaps and recommended remediation, providing reliable evidence of IT-dependent controls that allowed external financial auditors to place reliance on system-generated data and streamline audit procedures.
- **Data Integrity & Documentation:** Performed data integrity testing on key financial applications, including three-way match reconciliations using SQL and Excel, to validate the reliability of financial data and support timely completion of statutory audits. Updated and organised process documentation from prior engagements, creating a structured reference library in accordance with department’s policy that improved knowledge sharing, staff onboarding, and departmental training.
- **Compliance and Control Testing:** Assessed privileged access rights and application security configurations during system reviews to ensure SOX compliance. Identified and facilitated the remediation of five high-priority access vulnerabilities, strengthening clients’ compliance posture and enhancing the overall control environment.
- **Project Management:** Contributed to a £3.4m data governance transformation programme, supporting KPMG Lighthouse experts and client teams in aligning data strategy with ISO 27001 and GDPR standards. Assisted with stakeholder communications by preparing presentations, Q&A logs, and progress reports, and processed project documentation for KPMG experts, helping ensure milestones were delivered on time, within budget, and in line with regulatory requirements.

## DATA ANALYTICS & RESEARCH PROJECTS
---
### Credit Risk Analysis and Modelling | United Kingdom | April 2026 – May 2026

- **Objective:** Develop a production‑grade credit risk framework aligned with Basel IRB standards to estimate Probability of Default (PD), Loss Given Default (LGD), and Exposure at Default (EAD) for consumer loan portfolios, and integrate them into an Expected Loss (EL) engine to support capital planning, stress testing, and risk‑based pricing.
- **Methodology:** 
  - **Data Processing:** Processed ~250k Lending Club loans (2017–2018) with 152 raw features; reduced to 34 predictive variables using VIF, Condition Index, WoE, and IV analysis. 
  - **PD Model:** Class‑weighted logistic regression optimised with Youden’s index for threshold selection. 
  - **LGD Model:** Two‑stage framework where Stage 1 (logistic regression) predicts recovery likelihood and Stage 2 (OLS) estimates recovery magnitude conditional on recovery.
  - **EAD Model:** Linear regression based on Credit Conversion Factor (CCF) approach.
  - **Validation:** Independently validated on a holdout set of 50k loans.
- **Result:** 
  - **PD Model:** ROC‑AUC = 0.77, Gini = 0.53, KS = 0.40, Recall = 72% – demonstrates strong default detection and ranking ability.
  - **LGD Model (Stage 1 – Recovery Classification):** ROC‑AUC = 0.72, Recall = 84% – effectively identifies recoverable default accounts.
  - **LGD Model (Stage 2 – Recovery Magnitude):** MAE = 0.03, RMSE = 0.05, R² = 0.02 – low prediction errors, though low R² reflects inherent noise in recovery outcomes.
  - **EAD Model:** R² = 0.35, MAE = 0.08, RMSE = 0.115 – solid predictive power for exposure at default, strong for retail portfolios.
  - **Holdout Validation:** Performance decay minimal across all components (ROC‑AUC Δ = 0.0039, MAE Δ ≤ 0.012) – confirms robust generalisation and no over-fitting.

### BI Analytics Project – Olist’s E-Commerce Platform (Brazil) | United Kingdom | October 2025 – October 2025

- **Objective:** Conducted a comprehensive Business Intelligence analysis of Olist’s e-commerce dataset (100,000+ orders, 2016–2018) to deliver actionable insights for improving sales, customer retention, and marketplace competitiveness.
- **Methodology & Scope:** Utilized Power BI, Python, and MySQL to analyse 12 relational tables and develop interactive dashboards for insights across operational performance, logistics, customer reviews, and lead conversion.
- **Results:**
    - Identified 55% revenue concentration in three product categories and a 93.6% one-time buyer rate, recommending loyalty programmes and category diversification to increase customer lifetime value by 10–15%.
    - Uncovered critical operational bottlenecks, including 2.8-day seller-to-carrier delays and regional delivery disparities; proposed a dual logistics strategy — centralized fulfilment hubs for high-volume regions (e.g. São Paulo) and decentralized partnerships for low-volume areas along with ML-driven predictive models to reduce fulfilment variance.

### Analytical Research Project – MSc Dissertation, University of Exeter | United Kingdom | July 2025 – September 2025

- **Objective:** Investigated the dynamic relationship between airport activity (passenger volumes and freight throughput) and regional economic productivity (GVA per head) across 12 UK ITL1 regions, testing for bidirectional causality to provide evidence-based insights informing the UK’s Levelling Up agenda, aviation policy, and regional development strategies.
- **Methodology:** Employed Panel Vector Autoregression (PVAR) and Granger causality tests on a balanced panel dataset (1998–2023, 312 observations) using R Studio, integrating UK Civil Aviation Authority (CAA) airport data with Office for National Statistics (ONS) regional GVA metrics; analysed impacts while controlling for population density, applying stationarity tests (Im-Pesaran-Shin), logarithmic transformations, and lag selection (AIC/SC) for robust econometric modelling..
- **Result:** 
    - Confirmed passenger activity Granger-causes productivity with short-term adjustment costs and medium-term gains (lag 2: +0.0183, p<0.01), driven by aircraft movements; freight responds to productivity growth (Z=3.382, p<0.01) but does not cause or drive it.
    - Recommended prioritizing flight frequency, route diversity, and efficiency in hub regions, while enhancing targeted connectivity in emerging regions to boost productivity.


## COMMUNITY SERVICE & EXTRA CURRICULAR ACTIVITIES
---

### Volunteer in various Food Action initiatives | United Kingdom | November 2024 – June 2025
- **Community Impact:** Collected and distributed an average of 285 meal portions per month to shelters and vulnerable individuals, addressing food-poverty issues and providing essential nutrition to the low-income community.
- **Logistics and Fair Distribution:** Managed food inventory, maintained accurate records, and prioritized distribution based on community needs, ensuring fair and needs-based meal distribution to shelters.
- **Event Support:** Assisted in charity event logistics, including venue setup and table preparation, creating welcoming environments that enhanced donor and guest experiences. Recognized as Top Volunteer at Food Action Exeter in Q4 2024 for exceptional contributions and dedication.

### Media & Events Assistant | CFA Community of Vietnam, Vietnam | February 2022 – July 2024
- **Event Delivery:** Assisted in organising 2 flagship events (Forecast Dinner, Charter Award Ceremony) with 100+ attendees, ensuring seamless execution and professional delivery.
- **Data-Driven Engagement:** Designed and analysed post-event surveys, improving topic relevance and driving a 7% increase in member engagement on the CFA Vietnam community page.
- **Content Management:** Managed digital communications, ensuring alignment with CFA standards and guideline.

---
## Skills
---
<p>
  <img src="https://img.shields.io/badge/SQL-Intermediate-4479A1?style=flat&logo=mysql&logoColor=white" alt="SQL Skill Badge">
</p>

<p>
  <img src="https://img.shields.io/badge/Power%20BI-Advanced-F2C811?style=flat&logo=powerbi&logoColor=white" alt="Power BI Skill Badge">
</p>

<p>
  <img src="https://img.shields.io/badge/Excel-Advanced-217346?style=flat&logo=microsoft-excel&logoColor=white" alt="Excel Skill Badge">
</p>

<p>
  <img src="https://img.shields.io/badge/Python-Intermediate-3776AB?style=flat&logo=python&logoColor=white" alt="Python Skill Badge">
</p>
- Pandas  
- NumPy  
- Matplotlib
- Seaborn  
- Scikit-learn  

<p>
  <img src="https://img.shields.io/badge/R-Intermediate-276DC3?style=flat&logo=r&logoColor=white" alt="R Skill Badge">
</p> 
- dplry
- ggplot2
- tidyr
- lmtest
- AER
- fGarch



<!--
Skills
======
* Skill 1
* Skill 2
  * Sub-skill 2.1
  * Sub-skill 2.2
  * Sub-skill 2.3
* Skill 3

Publications
======
  <ul>{% for post in site.publications reversed %}
    {% include archive-single-cv.html %}
  {% endfor %}</ul>
  
Talks
======
  <ul>{% for post in site.talks reversed %}
    {% include archive-single-talk-cv.html  %}
  {% endfor %}</ul>
  
Teaching
======
  <ul>{% for post in site.teaching reversed %}
    {% include archive-single-cv.html %}
  {% endfor %}</ul>
  
Service and leadership
======
* Currently signed in to 43 different slack teams
-->