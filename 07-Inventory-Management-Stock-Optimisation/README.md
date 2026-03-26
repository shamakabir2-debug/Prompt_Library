# 07 · Inventory Management and Stock Optimisation

**Current version:** 7.0

**Status:** Tested and approved

**Last updated:** March 2026

## Prompt Text (v7.0 - Current)

> Act as an inventory management analyst for the ShopGO e-commerce platform. Analyse the following product data, current inventory levels, and demand forecasts to optimise stock management.
>
> Provide:
> 1. Stock status (Overstocked / Optimal / Low Stock / Out of Stock)  
> 2. Recommended action (e.g., reorder, reduce stock, maintain current level)  
> 3. Brief justification based on demand trends and inventory levels  
>
> If the data is incomplete or inconsistent, classify the result as **"Review Required"**.
>
> **Data inputs:**  
> Current inventory levels: [Stock data]  
> Demand forecast: [Forecast data]  
> Product details: [Category, sales rate, lead time]

# Intended Workflow or Task

This prompt is part of the **inventory monitoring and stock optimisation workflow** in the ShopGO e-commerce platform.

- **Trigger:** Inventory levels are updated or periodic stock review is initiated  
- **Actor:** AI system analyses stock and demand; operations team reviews output  
- **Timing:** Daily monitoring or during replenishment planning cycles  
- **Next step:** Stock decision applied → reorder placed, stock reduced, or maintained  

Inventory data updated → [Inventory prompt runs] → Stock status determined → Action recommended → Inventory adjusted

---

# Problem Being Solved

Managing inventory across a large e-commerce platform is complex and requires continuous monitoring of stock levels and demand patterns.

In ShopGO, this leads to:
- Overstocking, resulting in increased holding costs and potential waste  
- Stockouts, leading to lost sales and poor customer experience  
- Inefficient inventory allocation across products  
- Delayed decision-making due to manual analysis  

**Pain points addressed:**
- Difficulty analysing large volumes of inventory data  
- Lack of real-time visibility into stock performance  
- Inconsistent decision-making across different products  
- Limited ability to align inventory with demand forecasts  

---

# Automation Potential

**Level: High**

| Dimension                | Assessment |
|------------------------|-----------|
| Repetitiveness         | High; required for continuous inventory monitoring |
| Data availability      | High; stock levels, forecasts, and product data available |
| Human judgement needed | Medium; required for strategic or high-impact decisions |
| Integration possibility| Can be integrated into inventory management and ERP systems |
| Estimated impact       | Reduced stockouts, lower holding costs, improved inventory efficiency |

---

**Human-in-the-loop role:**  
Operations or supply chain managers review recommendations for critical or high-value products, validate assumptions, and make final decisions on inventory adjustments.

---

**Scaling note:**  
ShopGO manages thousands of products across multiple categories. Automating inventory analysis enables consistent, real-time optimisation at scale, significantly improving efficiency and supporting data-driven supply chain decisions.

---

## Risks and Limitations

- Incorrect demand forecasts may lead to poor inventory decisions  
- Supply chain delays or sudden demand spikes may not be captured  
- AI may overlook strategic, seasonal, or contextual factors  
- Data inaccuracies can affect recommendation quality

## Key Insights

- The prompt provides a structured approach to evaluating inventory status, ensuring consistent decision-making across products  
- Integration of demand forecasts improves alignment between stock levels and expected sales  
- Clear classification of stock status (Overstocked, Optimal, Low Stock, Out of Stock) simplifies operational decision-making  
- Recommended actions directly support inventory optimisation, reducing both stockouts and excess inventory  
- The “Review Required” fallback ensures that incomplete or inconsistent data does not lead to incorrect decisions  
- The prompt enables proactive inventory management rather than reactive decision-making  

---

## Conclusion

This prompt demonstrates how combining inventory data with demand forecasts and structured decision logic can improve stock optimisation in an e-commerce environment. By enabling consistent, scalable, and data-driven inventory decisions, the system reduces operational inefficiencies, minimises costs, and enhances product availability. As a result, it supports more effective supply chain management within the ShopGO platform.
