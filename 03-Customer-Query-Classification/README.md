# 03 · Customer Query Classification
**Current version:** 3.1

**Status:** Tested and approved

**Last updated:** March 2026
## Prompt Text (v3.1 - Current)

> You are a customer support classification system for the ShopGO e-commerce platform. Analyse the following customer query and classify it into one of the predefined categories:
>
> - Delivery Issue  
> - Refund/Return Request  
> - Product Inquiry  
> - Order Issue  
> - Complaint  
> - General Inquiry  
>
> For the query, provide:
> 1. Category  
> 2. Urgency level (Low / Medium / High)  
> 3. A brief reason for the classification  
>
> If the query is unclear or does not fit any category, classify it as **"Review Required"**.
>
> **Customer query:** [customer’s message]

# Intended Workflow or Task

This prompt is part of the **customer support triage and ticket routing workflow** in the ShopGO e-commerce platform.

- **Trigger:** Customer submits a query via chat, email, or support form  
- **Actor:** AI system classifies query; support system routes ticket  
- **Timing:** Real-time upon query submission  
- **Next step:** Query is routed to the appropriate department → support agent responds  

Customer submits query → [Classification prompt runs] → Category + urgency assigned → Routed to correct team → Response initiated

---

# Problem Being Solved

Customer queries are often unstructured and received in high volumes, making manual classification inefficient.

In a large e-commerce platform like ShopGO, this leads to:
- Delays in response time  
- Incorrect routing of support tickets  
- Increased workload for support teams  
- Reduced customer satisfaction  

**Pain points addressed:**
- Lack of standardisation in query classification  
- Difficulty handling ambiguous or multi-intent queries  
- Inefficient prioritisation of urgent issues  
- High manual effort in sorting and routing tickets  

---

# Automation Potential

**Level: Very High**

| Dimension                | Assessment |
|------------------------|-----------|
| Repetitiveness         | Very high; required for every customer query |
| Data availability      | High; query text available at submission |
| Human judgement needed | Low; only for complex or unclear cases |
| Integration possibility| Can be integrated into helpdesk |
| Estimated impact       | Faster response time, improved routing accuracy, reduced workload |
| Time estimate          | Manual classification: 1–2 minutes per query, with AI: 2–5 seconds, time saved per query: 1–2 minutes, efficiency improvement: 90–95% (approx.) |


---

**Human-in-the-loop role:**  
Support agents handle queries classified as “Review Required” and manage complex or sensitive cases. They also monitor classification accuracy and provide feedback for system improvement.

---

**Scaling note:**  
ShopGO may receive thousands of customer queries daily. Automating classification enables real-time triage at scale, significantly improving response efficiency and maintaining service quality as the platform grows.

## Risks and Limitations

- Complex or vague queries may be incorrectly categorised  
- Incorrect urgency classification may delay critical issues  
- Over-reliance on automation may reduce human oversight in sensitive or high-risk cases  


# Version History — Customer Query Classification

---

## v3.0 — Initial draft

**Date:** 20 March 2025  

**Prompt:**  
Act as a customer support system for the ShopGO e-commerce platform. Analyse the following customer query and identify what the customer is asking for. Provide a category and urgency level.

Customer query: [customer’s message]

**Output:**  
Basic classification generated but inconsistent across queries. Categories varied and were not standardised.

**Observed effect:**  
Difficult to route queries automatically due to inconsistent labels. Some queries were misclassified or unclear.

**Lesson learned:**  
Need predefined categories, structured output, and fallback handling for unclear queries to enable reliable automation.

---

## v3.1 — Added predefined categories and fallback logic (Current)

**Date:** 25 March 2025  

**Change:**  
Introduced predefined categories, urgency level, structured output format, and “Review Required” fallback for ambiguous queries.

**Prompt:**  
You are a customer support classification system for the ShopGO e-commerce platform. Analyse the following customer query and classify it into one of the predefined categories: Delivery Issue, Refund/Return Request, Product Inquiry, Order Issue, Complaint, General Inquiry.

For the query, provide:  
(1) category,  
(2) urgency level (Low/Medium/High), and  
(3) a brief reason for classification.  

If the query is unclear or does not fit any category, classify it as “Review Required.”  

Customer query: [customer’s message]

**Output:**  
Consistent and structured classification across queries. Improved clarity and routing accuracy.

**Observed effect:**  
Significantly improved automation of ticket routing and prioritisation. Reduced manual sorting effort.

**Lesson learned:**  
Predefined categories and fallback logic are essential for consistent classification and scalable workflow automation.

---

# A/B Test Results

**Test date:** 26 March 2025  
**Evaluators:** 4 customer support analysts 

| Criteria                      | v1.0 Score | v1.1 Score |
|-----------------------------|-----------|-----------|
| Classification Accuracy     | 2.5/5     | 4.6/5     |
| Consistency of Labels       | 2/5       | 4.7/5     |
| Handling Ambiguous Queries  | 1/5       | 4.8/5     |
| Routing Effectiveness       | 2/5       | 4.6/5     |
| Automation Readiness        | 1.5/5     | 4.5/5     |
| **Overall**                 | **1.8/5** | **4.6/5** |

---

## Key Insights

- v3.0 produced inconsistent and non-standard categories, limiting automation capability  
- v3.1 significantly improved classification accuracy through predefined categories  
- Introduction of “Review Required” improved handling of ambiguous queries  
- Structured output enabled direct integration into ticket routing systems  
- v3.1 reduced manual workload and improved response prioritisation  

---

## Conclusion

The transition from v3.0 to v3.1 demonstrates that structured classification rules and fallback logic are critical for reliable customer support automation. These improvements enhance consistency, scalability, and operational efficiency in real-world e-commerce environments.

