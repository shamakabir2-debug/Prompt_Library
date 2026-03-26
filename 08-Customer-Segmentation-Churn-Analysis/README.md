# 08 · Customer Segmentation and Churn Rate Analysis

**Current version:** 8.0

**Status:** Tested and approved

**Last updated:** March 2026

## Prompt Text (v8.0 - Current)

> Act as a customer analytics specialist for the ShopGO e-commerce platform. Analyse the following customer data to segment users into meaningful groups and identify their churn risk.
>
> Provide:
> 1. Customer segment (e.g., high-value, frequent buyer, occasional shopper, at-risk customer)  
> 2. Churn risk level (Low / Medium / High)  
> 3. Key reasons for classification (e.g., reduced purchase frequency, declining engagement, low spending)  
>
> If the data is insufficient or inconsistent, classify the result as **"Review Required"**.
>
> **Customer data:**  
> Purchase history: [Transaction data]  
> Browsing behaviour: [Activity data]  
> Engagement metrics: [Frequency, recency, spending]

# Intended Workflow or Task

This prompt is part of the **customer analytics and retention strategy workflow** in the ShopGO e-commerce platform.

- **Trigger:** Periodic customer analysis or decline in engagement detected  
- **Actor:** AI analyses customer data; marketing/CRM team reviews output  
- **Timing:** Weekly or monthly analytics cycle  
- **Next step:** Segments identified → churn risk assessed → targeted retention campaigns executed  

Customer data collected → [Segmentation prompt runs] → Segment + churn risk assigned → Insights generated → Retention actions implemented

---

# Problem Being Solved

E-commerce platforms manage diverse customer bases with varying behaviours, making it difficult to identify at-risk users and tailor engagement strategies.

In ShopGO, this leads to:
- High customer churn rates  
- Ineffective marketing campaigns  
- Missed opportunities for retention and upselling  
- Poor understanding of customer behaviour patterns  

**Pain points addressed:**
- Lack of structured customer segmentation  
- Difficulty identifying early signs of churn  
- Inefficient targeting of marketing efforts  
- Limited use of behavioural data for decision-making  

---

# Automation Potential

**Level: High**

| Dimension                | Assessment |
|------------------------|-----------|
| Repetitiveness         | High; required for regular customer analysis |
| Data availability      | High; purchase, browsing, and engagement data available |
| Human judgement needed | Medium; strategic decisions require human input |
| Integration possibility| Can be integrated into CRM and marketing systems |
| Estimated impact       | Improved retention, better targeting, increased customer lifetime value |

---

**Human-in-the-loop role:**  
Marketing and CRM teams review segmentation outputs, validate insights, and design targeted campaigns or retention strategies.

---

**Scaling note:**  
ShopGO serves a large customer base with varying behaviours. Automating segmentation enables consistent analysis across thousands of users, supporting personalised engagement and scalable retention strategies.

---
## Risks and Limitations

- Use of customer behavioural data must comply with data protection and privacy regulations  
- Over-generalising segments may oversimplify complex customer behaviour  
- Incomplete or outdated data may affect segmentation accuracy  
- AI may not fully capture qualitative factors influencing customer behaviour

## Key Insights

- The prompt enables structured customer segmentation, improving understanding of user behaviour patterns  
- Integration of churn risk assessment allows early identification of at-risk customers  
- Use of behavioural indicators (frequency, recency, spending) enhances accuracy of classification  
- Clear segmentation supports targeted marketing and personalised engagement strategies  
- The “Review Required” fallback ensures uncertain cases are handled carefully  
- The prompt supports proactive retention rather than reactive customer recovery  

---

## Conclusion

This prompt demonstrates how structured customer data analysis can improve segmentation and churn prediction in an e-commerce environment. By enabling consistent classification and early identification of at-risk users, the system supports targeted retention strategies, enhances customer lifetime value, and improves overall business performance within the ShopGO platform.
