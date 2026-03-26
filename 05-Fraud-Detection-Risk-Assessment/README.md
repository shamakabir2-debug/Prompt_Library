# 05 · Fraud Detection and Risk Assessment

**Current version:** 5.0

**Status:** Tested and approved

**Last updated:** March 2026
## Prompt Text (v5.0 - Current)

> You are a fraud detection and risk assessment system for the ShopGO e-commerce platform. Analyse the following transaction and customer activity data to identify potential signs of fraud.
>
> Provide:
> 1. Fraud risk level (Low / Medium / High)  
> 2. Key risk indicators (e.g., unusual purchase behaviour, multiple failed payments, location mismatch, false personal details, suspicious IP address)  
> 3. Recommended action (Approve / Flag for review / Block transaction)  
>
> If the data is insufficient or inconclusive, classify the case as **"Review Required"**.
>
> **Transaction details:** [Transaction data]  
> **Customer activity:** [Browsing, login, and purchasing patterns]

# Intended Workflow or Task

This prompt is part of the **transaction monitoring and fraud prevention workflow** in the ShopGO e-commerce platform.

- **Trigger:** Customer initiates or completes a transaction  
- **Actor:** AI system evaluates transaction; security system enforces action  
- **Timing:** Real-time during checkout or immediately after payment  
- **Next step:** Transaction is approved, flagged for manual review, or blocked  

Customer places order → [Fraud detection prompt runs] → Risk level assessed → Action triggered → Transaction processed or escalated

---

# Problem Being Solved

E-commerce platforms are highly vulnerable to fraudulent activities such as unauthorised transactions, identity misuse, and payment fraud.

In a platform like ShopGO, this leads to:
- Financial losses from fraudulent transactions  
- Chargebacks and increased operational costs  
- Damage to brand trust and customer confidence  
- Security risks affecting both customers and the platform  

**Pain points addressed:**
- Difficulty identifying fraud in real time  
- High volume of transactions making manual review impractical  
- Inconsistent fraud detection across different cases  
- Need to balance fraud prevention with customer experience  

---

# Automation Potential

**Level: Very High**

| Dimension                | Assessment |
|------------------------|-----------|
| Repetitiveness         | Very high; required for every transaction |
| Data availability      | High; transaction and behavioural data available |
| Human judgement needed | Medium; required for flagged or complex cases |
| Integration possibility| Can be integrated into payment and security systems |
| Estimated impact       | Reduced fraud losses, improved security, faster decision-making |

---

**Human-in-the-loop role:**  
Fraud analysts review transactions flagged as “Review Required” or high-risk cases to make final decisions and handle disputes or edge cases.

---

**Scaling note:**  
ShopGO processes a large volume of transactions daily. Automating fraud detection enables real-time risk assessment at scale, ensuring consistent protection while maintaining efficient transaction processing.

## Risks and Limitations

- Legitimate transactions may be incorrectly flagged (false positives)  
- Fraudulent transactions may go undetected (false negatives)  
- Fraudsters may adapt their behaviour to bypass detection systems  
- Over-reliance on automation may reduce human judgement in complex cases

## Key Insights

- The prompt provides a structured framework for analysing transactions, ensuring consistent identification of fraud risk across all cases  
- Clearly defined risk indicators (e.g., suspicious IP address, location mismatch, repeated failed payments) improve detection accuracy and reduce ambiguity  
- The inclusion of risk levels (Low / Medium / High) enables prioritisation of cases and supports faster decision-making  
- Recommended actions (Approve / Flag / Block) directly align with operational workflows, enabling seamless integration into transaction systems  
- The “Review Required” fallback ensures that incomplete or inconclusive data does not result in incorrect automated decisions  
- The prompt balances automation with control, allowing high-volume transaction processing while maintaining safeguards for edge cases  

---

## Conclusion

This prompt demonstrates how structured inputs, clearly defined risk indicators, and decision-oriented outputs can enable effective fraud detection in an e-commerce environment. By combining real-time analysis with fallback handling, the system supports accurate, scalable, and consistent transaction monitoring. As a result, the prompt enhances security, reduces financial risk, and improves operational efficiency within the ShopGO platform.
