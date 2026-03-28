# Prompt Library — ShopGO E-commerce Workflow Automation

**Assessment 1 | Generative AI for Business**  

**Student:** Shama Kabir 

**Business Field:** E-commerce & Online Retail Operations 

**Model tested on:** La Trobe University Prompt Lab | GPT-4.1 Mini

**Last updated:** March 2026  

---

# What This Library Does

This prompt library supports workflow automation in the **ShopGO e-commerce platform**. It contains **10 documented, tested, and iterated prompts** designed to improve operational efficiency, decision-making, and customer experience.

Each prompt follows a consistent structure:
- Prompt text (with placeholders)
- Intended workflow or task
- Problem being solved
- Automation potential
- Risks and limitations
- Version history and A/B testing results

---

# Library Summary Table

| ID  | Prompt Name                        | Workflow              | Automation Level | Risk Level | Status |
|-----|----------------------------------|----------------------|------------------|-----------|--------|
| P01 | Product Title & SEO              | Product listing      | High             | Low       | ✅ Tested |
| P02 | Personalised Recommendation      | Product discovery    | Very High        | Medium    | ✅ Tested |
| P03 | Customer Query Classification    | Customer support     | Very High        | Medium    | ✅ Tested |
| P04 | Refund/Return Evaluation         | Customer support     | High             | Medium    | ✅ Tested |
| P05 | Fraud Detection                 | Risk & security      | Very High         | High      | ✅ Tested |
| P06 | Sales & Demand Forecasting       | Analytics            | High             | Medium    | ✅ Tested |
| P07 | Inventory Optimisation           | Operations           | High             | Medium    | ✅ Tested |
| P08 | Customer Segmentation            | Analytics            | High             | Medium    | ✅ Tested |
| P09 | Sentiment Analysis               | Feedback analysis    | Very High        | Low       | ✅ Tested |
| P10 | Marketing Email Generation       | Marketing            | Very High        | Low       | ✅ Tested |

---

# Prompt Chaining Map

Some prompts are designed to work sequentially across workflows:

### Customer Journey Chain
P01 (Product Title SEO) → P02 (Recommendation) → P10 (Marketing Email)

### Customer Support Chain
P03 (Query Classification) → P04 (Refund Evaluation)

### Operations Chain
P06 (Demand Forecasting) → P07 (Inventory Optimisation)

### Customer Intelligence Chain
P08 (Segmentation) → P09 (Sentiment Analysis)

---

# Prompting Strategies Used

| Strategy | Prompts | Why chosen |
|----------|--------|------------|
| Role-based prompting | All | Ensures consistent and context-aware outputs |
| Structured outputs | P03, P04, P05, P06 | Enables automation and system integration |
| Fallback logic | P02, P03, P04, P05 | Handles missing or ambiguous data |
| Constraints (word limits, format) | P01, P10 | Ensures production-ready outputs |
| Data grounding ("use only provided data") | P05, P06 | Reduces hallucination |
| Explainability (reason/justification) | Most prompts | Improves transparency and trust |

---

# Iteration Evidence

All prompts were iteratively refined based on testing and evaluation.

| Prompt | Versions | Key Improvement |
|--------|---------|----------------|
| P02 Recommendation | v2.0 → v2.1 | Added fallback logic for first-time users |
| P03 Classification | v3.0 → v3.1 | Introduced predefined categories + consistency |
| P06 Forecasting | v6.0 → v6.1 | Added drivers and confidence handling |
| P10 Marketing Email | v10.0 → v10.1 | Added structure (subject, body) and tone |

