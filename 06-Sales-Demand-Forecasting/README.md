# 06 · Sales and Demand Forecasting

**Current version:** 6.1

**Status:** Tested and approved

**Last updated:** March 2026

## Prompt Text (v6.1 - Current)

> Act as a sales and demand forecasting analyst for the ShopGO e-commerce platform. Analyse the following historical sales data, seasonal trends, and product performance information to predict future demand.
>
> Provide:
> 1. Forecasted demand for the next period (e.g., week/month)  
> 2. Key factors influencing demand (e.g., seasonality, promotions, trends)  
> 3. Recommended actions (e.g., increase inventory, adjust pricing, run promotions)  
>
> If the data is insufficient or inconsistent, classify the forecast as **"Low Confidence"** and explain why.
>
> **Data inputs:**  
> Historical sales data: [Past sales figures]  
> Seasonal trends: [Seasonal patterns]  
> Product performance: [Product metrics]

# Intended Workflow or Task

This prompt is part of the **sales forecasting and inventory planning workflow** in the ShopGO e-commerce platform.

- **Trigger:** Periodic analysis (daily/weekly/monthly) or planning cycle  
- **Actor:** AI generates forecast; operations team reviews insights  
- **Timing:** Before inventory replenishment or promotional planning  
- **Next step:** Forecast used for stock planning, pricing decisions, and marketing strategies  

Sales data collected → [Forecasting prompt runs] → Demand forecast generated → Business actions planned → Inventory and pricing adjusted

---

# Problem Being Solved

Accurate demand forecasting is critical for efficient e-commerce operations. Without reliable forecasts, businesses struggle to balance supply and demand.

In ShopGO, this leads to:
- Overstocking (increased holding costs and waste)  
- Stockouts (lost sales and poor customer experience)  
- Ineffective promotional planning  
- Poor pricing decisions  

**Pain points addressed:**
- Difficulty analysing large volumes of sales data  
- Lack of structured forecasting insights  
- Inability to identify key demand drivers  
- Limited decision support for operations teams  

---

# Automation Potential

**Level: High**

| Dimension                | Assessment |
|------------------------|-----------|
| Repetitiveness         | High; required for regular planning cycles |
| Data availability      | High; historical and performance data available |
| Human judgement needed | Medium; strategic decisions require human input |
| Integration possibility| Can be integrated into analytics and planning systems |
| Estimated impact       | Improved inventory planning, reduced costs, increased sales |

---

**Human-in-the-loop role:**  
Operations and analytics teams review forecasts, validate assumptions, and make final strategic decisions such as pricing and promotions.

---

**Scaling note:**  
ShopGO manages a large and dynamic product catalogue. Automating demand forecasting enables consistent analysis across thousands of products, improving operational efficiency and supporting data-driven decision-making at scale.


## Risks and Limitations

- Sudden market changes (e.g., trends, supply disruptions) may not be captured  
- Past patterns may not always reflect future behaviour  
- AI may oversimplify complex demand patterns  
- Data quality issues can reduce forecast accuracy

# Version History — Sales and Demand Forecasting

---

## v6.0 — Initial draft

**Date:** 19 March 2025  

**Prompt:**  
Act as a sales analyst for the ShopGO e-commerce platform. Analyse the sales data and predict future demand. Provide a forecast and explain the results.

Data: [Sales data]

**Output:**  
General predictions provided, but lacked structure and consistency. Limited explanation of key drivers.

**Observed effect:**  
Outputs were vague and difficult to use for decision-making. Recommendations were often generic and not actionable.

**Lesson learned:**  
Need structured outputs, clearer inputs, and actionable recommendations to support real business decisions.

---

## v6.1 — Added structure, drivers, and confidence handling (Current)

**Date:** 24 March 2025  

**Change:**  
Introduced structured outputs, included demand drivers (seasonality, trends), and added “Low Confidence” handling for insufficient data.

**Prompt:**  
Act as a sales and demand forecasting analyst for the ShopGO e-commerce platform. Analyse the following historical sales data, seasonal trends, and product performance information to predict future demand.  

Provide:  
(1) Forecasted demand for the next period (e.g., week/month),  
(2) Key factors influencing demand (e.g., seasonality, promotions, trends), and  
(3) Recommended actions (e.g., increase inventory, adjust pricing, run promotions).  

If the data is insufficient or inconsistent, classify the forecast as “Low Confidence” and explain why.  

Data inputs:  
- Historical sales data: [Past sales figure]  
- Seasonal trends: [Seasonal patterns]  
- Product performance: [Product metrics]  

**Output:**  
Structured forecasts with clear drivers and actionable recommendations.

**Observed effect:**  
Improved usability for inventory planning and business decisions. Outputs became more consistent and reliable.

**Lesson learned:**  
Structured outputs and confidence indicators are essential for making forecasts actionable and trustworthy.

---

# A/B Test Results

**Test date:** 26 March 2025  
**Evaluators:** 3 e-commerce operations analysts 

| Criteria                          | v1.0 Score | v1.1 Score |
|----------------------------------|-----------|-----------|
| Forecast Clarity                 | 2/5       | 4.6/5     |
| Actionability of Output          | 1.5/5     | 4.7/5     |
| Identification of Key Drivers    | 1/5       | 4.6/5     |
| Consistency of Results           | 2/5       | 4.5/5     |
| Decision Support Usefulness      | 1.5/5     | 4.7/5     |
| **Overall**                      | **1.6/5** | **4.6/5** |

---

## Key Insights

- v6.0 produced vague forecasts with limited practical value  
- v6.1 significantly improved clarity and usefulness through structured outputs  
- Inclusion of key demand drivers enhanced understanding of forecast results  
- “Low Confidence” handling improved reliability in uncertain scenarios  
- v6.1 outputs were directly usable for inventory and pricing decisions  

---

## Conclusion

The improvements from v6.0 to v6.1 demonstrate that structured outputs, inclusion of demand drivers, and confidence handling significantly enhance the usefulness and reliability of forecasting prompts. These enhancements make the system suitable for real-world decision-making and scalable automation.

