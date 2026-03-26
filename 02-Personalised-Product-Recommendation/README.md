# 02 · Personalised Product Recommendation

**Current version:** v2.1

**Status:** Tested and approved

**Last updated:** March 2026



## Prompt Text (v2.1 - Current)

> Act as a recommendation engine for the ShopGO e-commerce platform. Based on the customer’s browsing history, past purchases, and stated preferences, suggest 5 personalised products.  
>
> If customer data is unavailable (first-time user), recommend products based on trending items, high ratings, and popular categories.  
>
> Ensure the recommendations are relevant, diverse, and aligned with customer interests.

# Intended Workflow or Task

This prompt is part of the **product discovery and recommendation workflow** in the ShopGO e-commerce platform.

- **Trigger:** Customer visits homepage or product page  
- **Actor:** Recommendation system (AI generates suggestions), platform displays results  
- **Timing:** Real-time during browsing session  
- **Next step:** Recommended products are displayed → customer clicks → proceeds to product page or checkout  

Customer visits platform → [Recommendation prompt runs] → Product suggestions generated → Displayed to user → Customer interaction (click/purchase)

---

# Problem Being Solved

Customers are exposed to a large number of products, making it difficult to quickly identify relevant items.

In a large-scale e-commerce platform like ShopGO, this leads to:
- Low product discovery efficiency  
- Reduced engagement and session time  
- Missed cross-selling and upselling opportunities  

**Pain points addressed:**
- Lack of personalisation for returning users  
- No recommendation support for first-time users 
- Repetitive or irrelevant product suggestions  
- Reduced conversion rates due to poor product visibility  

---

# Automation Potential

**Level: Very High**

| Dimension                | Assessment |
|------------------------|-----------|
| Repetitiveness         | Very high; recommendation required for every user session |
| Data availability      | High; browsing history, purchase data, and preferences available |
| Human judgement needed | Very low; monitoring only |
| Integration possibility| Can be embedded in website/app recommendation engine |
| Estimated impact       | Increased engagement, improved customer experience |

---

**Human-in-the-loop role:**  
Product and analytics teams monitor recommendation performance and refine logic, but no manual intervention is required for each recommendation.

---

**Scaling note:**  
System can generate recommendations for thousands of users simultaneously in real time, significantly improving scalability compared to manual or rule-based systems.

## Risks and Limitations

- Use of customer behaviour data must comply with privacy regulations  
- Over-personalisation may limit product discovery and reduce exposure to new items  
- Recommendations may be inaccurate if customer data is incomplete or outdated

## Version History 
## v2.0 — Initial draft

**Date:** 20 March 2026  

**Prompt:**  
Act as a recommendation system for the ShopGO e-commerce platform. Based on the customer’s browsing history, past purchases, and preferences, suggest 5 products that the customer may be interested in. Ensure the recommendations are relevant.

**Output:**  
Basic recommendations generated but lacked diversity and consistency. Did not account for users with no prior data.

**Observed effect:**  
Limited usefulness in real scenarios — failed to generate recommendations for first-time users and produced repetitive or overly similar products.

**Lesson learned:**  
Need to handle missing data, include diversity constraints, and improve recommendation logic for realistic automation.

---

## v2.1 — Added fallback logic and diversity rules (Current version)

**Date:** 25 March 2026  

**Change:**  
Added condition for first-time users using trending products and high ratings. Included requirement for diverse recommendations.

**Prompt:**  
Act as a recommendation engine for the ShopGO e-commerce platform. Based on the customer’s browsing history, past purchases, and stated preferences, suggest 5 personalised products. If customer data is unavailable (first-time user), recommend products based on trending items, high ratings, and popular categories. Ensure the recommendations are relevant, diverse, and aligned with customer interests.

**Output:**  
More realistic recommendations; system able to generate results for all users including first-time visitors. Improved variety in suggested products.

**Observed effect:**  
Recommendation quality improved significantly and became applicable in real-world scenarios. Reduced gaps in automation.

**Lesson learned:**  
Fallback logic is essential for scalability. Diversity improves recommendation quality and user engagement.

# A/B Test Results

**Test date:** 26 March 2025  
**Evaluators:** 3 e-commerce operations analysts 

| Criteria                          | v2.0 Score | v2.1 Score |
|----------------------------------|-----------|-----------|
| Relevance of Recommendations     | 2.5/5     | 4.6/5     |
| Diversity of Recommendations     | 1.5/5     | 4.5/5     |
| Handling of Missing Data         | 0/5       | 4.8/5     |
| Consistency of Output            | 2/5       | 4.4/5     |
| Practical Usefulness             | 2/5       | 4.6/5     |
| **Overall**                      | **1.6/5** | **4.6/5** |

---

## Key Insights

- v2.0 failed to handle first-time users, resulting in no or poor recommendations (score: 0/5 in missing data handling)  
- v2.1 introduced fallback logic, enabling recommendations even without prior customer data  
- Recommendation diversity improved significantly, reducing repetitive suggestions  
- Outputs became more consistent and aligned with real customer behaviour  
- v2.1 outputs were directly usable in workflow systems with minimal adjustment  

---

## Conclusion

The improvement from v2.0 to v2.1 highlights the importance of fallback logic and clearer instruction design in recommendation systems. These enhancements significantly improved relevance, robustness, and real-world applicability, making the prompt suitable for scalable e-commerce automation.
