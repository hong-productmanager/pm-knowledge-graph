---
tags: [execution, technical, risk]
type: concept
branch: 06 - Execution & Delivery
related: ["Model Drift & Degradation", "Data Quality", "Release Management"]
created: 2026-05-05
---

# Technical Debt in AI

## Definition
The accumulation of hidden costs in an AI system that arise from the unique properties of machine learning. It is categorized into four main types: **Model Debt** (using outdated architectures), **Data Debt** (stale training data), **Annotation Debt** (evolving label definitions), and **Monitoring Debt** (lack of visibility into production performance).

## How to Apply It
1. Audit Model Freshness: Regularly check if your model's performance on current real-world data matches its training performance.
2. Track Label Consistency: Ensure that if you change how you label data today, your historical data is also updated or re-evaluated.
3. Automate Monitoring: Invest in "Alerting" for when model confidence or accuracy drops below a certain threshold in production.
4. Plan for Model Sunset: Define when a model is "too old" and must be replaced by a newer architecture.

## Connected Concepts
- [[03 - AI & ML Fundamentals/Model Drift & Degradation]] — is the most common symptom of technical debt in AI
- [[04 - Data Strategy/Data Quality]] — is the primary prevention against "Data Debt"
- [[06 - Execution & Delivery/Release Management]] — provides the framework for deploying "fixes" to AI debt
