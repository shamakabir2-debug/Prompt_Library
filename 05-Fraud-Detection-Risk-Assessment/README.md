# 05 · Fraud Detection and Risk Assessment

## Prompt Text

> You are a fraud detection and risk assessment system for the ShopGO e-commerce platform. Analyse the following transaction and customer activity data to identify potential signs of fraud.
>
> Provide:
> 1. Fraud risk level (Low / Medium / High)  
> 2. Key risk indicators (e.g., unusual purchase behaviour, multiple failed payments, location mismatch, false personal details, suspicious IP address)  
> 3. Recommended action (Approve / Flag for review / Block transaction)  
>
> If the data is insufficient or inconclusive, classify the case as **"Review Required"**.
>
> **Transaction details:** [Insert transaction data]  
> **Customer activity:** [Insert browsing, login, and purchasing patterns]

## Intended Workflow or Task

This prompt is used during transactions to assess fraud risk and support real-time decision-making within the ShopGO platform.

## Problem Being Solved

E-commerce platforms face significant financial and reputational risks from fraudulent transactions. Manual fraud detection is inefficient and cannot keep up with high transaction volumes, increasing the likelihood of undetected fraud and financial loss.

## Automation Potential

**High.**  
Fraud detection can be integrated into real-time transaction systems to automatically assess risk levels. Human review is required for flagged or ambiguous cases.

## Risks and Limitations

- Legitimate transactions may be incorrectly flagged (false positives)  
- Fraudulent transactions may go undetected (false negatives)  
- Fraudsters may adapt their behaviour to bypass detection systems  
- Over-reliance on automation may reduce human judgement in complex cases  
