---
title: "Portfolio 1: Airport Activity and Regional Productivity in the United Kingdom: An Empirical Study of Connectivity, Freight Operations, and Economic Growth (1998–2023)"
excerpt: "This project analyzes the relationship between airport activity and regional economic productivity across the UK’s 12 ITL1 regions (1998–2023) using Panel Vector Autoregression (PVAR) and Granger causality analysis, providing evidence-based insights to guide aviation policy, regional development, and infrastructure investment decisions.<br/><img src='/images/Dissertation (Granger Causality).png'>"
collection: portfolio
---

📎For more details, click [here](https://github.com/Danny-NG-9999/Academic-and-Personal-Projects/tree/main/Dissertation%20Project)


## 🎯 Objective
The project aimed to quantify the dynamic relationship between airport activity and regional economic productivity across the UK’s 12 ITL1 regions from 1998 to 2023. Employing a Panel Vector Autoregression (PVAR) framework alongside Granger causality analysis, the study explored how passenger volumes and freight throughput influence Gross Value Added (GVA) per head — the primary productivity measure for this study.

The overarching goal was to deliver evidence-based insights to inform aviation policy, regional development strategy, and infrastructure investment decisions, clarifying whether airports function primarily as drivers of economic growth or as responders to regional economic performance in the UK context


## ⚙️ Tasks
- Data Collection & Preparation: Assembled a balanced panel dataset (1998–2023, 312 observations) integrating ONS Regional Accounts (GVA per head, population density) and CAA airport data (passenger volumes, freight, ATMs) for 12 ITL1 regions, focusing on top three airports per region. Applied logarithmic transformations and Im-Pesaran-Shin stationarity tests.
- Econometric Analysis: Utilized R Studio to implement Panel Vector Autoregression (PVAR), Dumitrescu-Hurlin Granger causality tests, and Impulse Response Functions (IRFs), with lag selection via AIC and Schwarz criteria, to model dynamic interactions between airport activity and productivity.
- Policy Formulation: Developed evidence-based recommendations to optimize aviation infrastructure investments based on findings.

## 💡 Results

**1️⃣ Passenger Activity — Productivity Driver**
- Causality: Passenger volumes Granger-cause regional productivity (Z = 23.143, p < 0.001).
- Short-Term Impact: Slight negative adjustment (–0.0335), reflecting congestion and transition costs.
- Medium-Term Impact: Positive productivity gains (+0.0183) emerge after 1–2 years as connectivity benefits materialize.
- Key Factor: Aircraft movements (ATMs) have a stronger influence than passenger volume alone, highlighting flight frequency and connectivity quality over passengers volume.

**2️⃣ Freight Activity — Productivity Responder**
- Causality: Productivity drives freight growth (Z = 3.382, p < 0.01); freight does not Granger-cause productivity.
- Reflects the UK’s service-based economy, where air cargo expands in response to economic activity rather than stimulating it.
- Freight growth typically lags productivity increases by ~2 years.

| Relationship             | Causality  |
| ------------------------ | -----------|
| Passenger → Productivity | ✅ Yes     |
| Productivity → Passenger | ❌ No      |
| Freight → Productivity   | ❌ No      |
| Productivity → Freight   | ✅ Yes     |

**3️⃣ Strategic Implications**
- Invest in network reliability and route frequency, not just airport capacity.
- Treat airports as connectivity enablers, not standalone growth engines.
- Align freight infrastructure with productive regions rather than using it to initiate growth.
- For major hubs (e.g., LHR, MAN, EDI): focus on operational efficiency and sustainability.
- For emerging regions: prioritize route diversification to enhance regional inclusion.

Overall, airports in the UK act as catalysts for regional productivity through enhanced connectivity — but only when integrated with strong regional economic structures. Their economic value is contingent on operational quality, network diversity, and alignment with regional strengths, rather than sheer volume growth.