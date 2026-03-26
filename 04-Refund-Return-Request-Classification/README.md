# 04 · Refund or Return Request Evaluation

**Current version:** 4.0

**Status:** Tested and approved

**Last updated:** March 2026

## Prompt Text (v4.0 - Current)

> Act as a returns and refund decision-support system for the ShopGO e-commerce platform. Evaluate the following customer request against the company’s return and refund policy.
>
> Provide:
> 1. Decision (Approve / Reject / Review)  
> 2. Reason for the decision (with reference to policy rules)  
> 3. Recommended next action (e.g., issue refund, request more information, arrange return)  
>
> If the information is incomplete or unclear, classify the request as **"Review Required"**.
>
> **Customer request:** [Request details]  
> **Return policy:** [Company policy rules]

# Intended Workflow or Task

This prompt is part of the **returns and refund processing workflow** in the ShopGO e-commerce platform.

- **Trigger:** Customer submits a refund or return request  
- **Actor:** AI evaluates request; support system processes outcome  
- **Timing:** Immediately after request submission  
- **Next step:** Decision is generated → action taken (refund issued, return initiated, or case escalated)

Customer submits request → [Refund evaluation prompt runs] → Decision generated → Action executed → Case resolved or escalated

---

# Problem Being Solved

Refund and return requests are often reviewed manually, leading to inconsistent decisions and delays.

In a large e-commerce platform like ShopGO, this results in:
- Slow response times  
- Inconsistent application of return policies  
- Increased operational costs  
- Customer dissatisfaction due to delayed or unfair decisions  

**Pain points addressed:**
- Manual interpretation of return policies  
- Lack of consistency across different support agents  
- Difficulty handling incomplete or unclear requests  
- Inefficient processing of high request volumes  

---

# Automation Potential

**Level: High**

| Dimension                | Assessment |
|------------------------|-----------|
| Repetitiveness         | High; frequent return/refund requests |
| Data availability      | High; request details and policy rules available |
| Human judgement needed | Medium; required for complex cases and disputes |
| Integration possibility| Can be integrated into returns management system |
| Estimated impact       | Faster processing, improved consistency, reduced workload |

---

**Human-in-the-loop role:**  
Support agents review cases classified as “Review Required” and handle exceptions, disputes, or cases requiring subjective judgement.

---

**Scaling note:**  
ShopGO processes large volumes of return and refund requests daily. Automating evaluation enables consistent, policy-based decisions at scale while reducing manual workload and improving customer experience.

## Risks and Limitations

- AI may misinterpret situations and apply incorrect policy rules  
- Incorrect approvals may result in financial loss  
- Unusual or edge-case scenarios may not fit predefined rules and require human judgement

## Key Insights

- The prompt applies structured decision logic (Approve / Reject / Review), ensuring consistent evaluation of refund requests  
- Referencing return policy rules improves transparency and reduces subjective decision-making  
- Recommended actions align directly with operational workflows, enabling efficient case handling  
- The “Review Required” fallback ensures incomplete or unclear cases are safely escalated rather than incorrectly processed  
- The prompt reduces variability across support agents, improving fairness and consistency in customer service  

---

## Conclusion

This prompt highlights the importance of policy-driven decision-making in refund and return processes. By combining structured outputs with clear policy references and fallback handling, the system enables consistent, scalable, and efficient evaluation of customer requests. This improves operational efficiency, reduces errors, and enhances customer trust in the ShopGO platform.
