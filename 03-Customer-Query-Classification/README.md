# 03 · Customer Query Classification

## Prompt Text

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
> **Customer query:** [Insert customer’s message]

## Intended Workflow or Task

This prompt is used when customer queries are received through channels such as chat, email, or social media. It enables automatic classification and routing of queries to the appropriate department for faster handling.

## Problem Being Solved

Customer queries are often unstructured and received in high volumes, making manual classification slow and inefficient. Delays in identifying the type and urgency of queries can result in slower response times, increased operational costs, and reduced customer satisfaction.

## Automation Potential

**Very High.**  
This task can be fully automated and integrated into customer support systems to enable real-time classification and routing of customer queries.

## Risks and Limitations

- Complex or vague queries may be incorrectly categorised  
- Incorrect urgency classification may delay critical issues  
- Over-reliance on automation may reduce human oversight in sensitive or high-risk cases  
