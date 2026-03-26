# 09 · Customer Review Sentiment Analysis

**Current version:** 9.0

**Status:** Tested and approved

**Last updated:** March 2026
## Prompt Text (v9.0 - Current)

> Act as a customer feedback analysis system for the ShopGO e-commerce platform. Analyse the following customer review and identify:
>
> 1. Overall sentiment (Positive / Negative / Neutral)  
> 2. Key issues or strengths mentioned  
> 3. Urgency level (Low / Medium / High) based on potential impact on customer satisfaction or brand reputation  
>
> If the review is unclear or lacks sufficient detail, classify it as **"Review Required"**.
>
> **Customer review:** [Review text]

# Intended Workflow or Task

This prompt is part of the **customer feedback analysis and quality improvement workflow** in the ShopGO e-commerce platform.

- **Trigger:** Customer submits a product review  
- **Actor:** AI analyses review; support/product team reviews insights  
- **Timing:** Real-time or batch processing of reviews  
- **Next step:** Insights generated → issues identified → actions taken (e.g., product improvement, support follow-up)  

Customer submits review → [Sentiment prompt runs] → Sentiment + issues identified → Insights generated → Actions taken

---

# Problem Being Solved

E-commerce platforms receive large volumes of customer reviews, making manual analysis time-consuming and inefficient.

In ShopGO, this leads to:
- Delayed identification of product or service issues  
- Missed opportunities for improvement  
- Inconsistent interpretation of customer feedback  
- Difficulty prioritising critical issues  

**Pain points addressed:**
- High volume of unstructured review data  
- Lack of systematic sentiment analysis  
- Difficulty identifying key issues and trends  
- Inefficient prioritisation of urgent feedback  

---

# Automation Potential

**Level: Very High**

| Dimension                | Assessment |
|------------------------|-----------|
| Repetitiveness         | Very high; required for every customer review |
| Data availability      | High; review text readily available |
| Human judgement needed | Low; only for high-urgency or unclear cases |
| Integration possibility| Can be integrated into review monitoring systems |
| Estimated impact       | Faster issue detection, improved product quality, enhanced customer experience |

---

**Human-in-the-loop role:**  
Support and product teams review high-urgency or flagged reviews, validate insights, and take corrective actions.

---

**Scaling note:**  
ShopGO receives thousands of customer reviews daily. Automating sentiment analysis enables real-time monitoring at scale, ensuring timely identification of issues and continuous improvement of products and services.

---

## Risks and Limitations

- Sarcasm, slang, or ambiguous language may reduce accuracy  
- AI may overemphasise certain keywords, leading to biased interpretations  
- Important nuanced feedback may be missed without human judgement  
- Context-specific meanings may not always be correctly interpreted

## Key Insights

- The prompt enables consistent sentiment classification across large volumes of reviews  
- Identification of key issues or strengths provides actionable insights for product and service improvement  
- Urgency classification helps prioritise critical feedback and allocate resources effectively  
- Structured outputs support integration into monitoring and analytics systems  
- The “Review Required” fallback ensures ambiguous or unclear reviews are handled appropriately  
- The prompt transforms unstructured feedback into meaningful, decision-ready insights  

---

## Conclusion

This prompt demonstrates how automated sentiment analysis can convert large volumes of customer feedback into actionable insights. By enabling consistent classification, prioritisation, and issue identification, the system supports continuous product improvement and enhances customer experience. As a result, it provides scalable and efficient feedback management within the ShopGO platform.
