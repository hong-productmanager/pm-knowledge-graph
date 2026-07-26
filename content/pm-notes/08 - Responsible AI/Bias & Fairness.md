---
tags: [responsible-ai, risk]
type: concept
branch: 08 - Responsible AI
related: ["Data Quality", "Transparency to Users", "Bias & Fairness"]
created: 2026-05-05
---

# Bias & Fairness

## Definition
Bias in AI occurs when a machine learning model produces results that are systematically prejudiced against certain groups of people, often due to historical inequities in the training data or flaws in the algorithm's design. **Fairness** is the practice of identifying, measuring, and mitigating these biases to ensure that the model's outcomes are equitable across all demographic groups (e.g., race, gender, age). Key concepts include **Group Fairness** (equal outcomes for groups) and **Individual Fairness** (similar individuals treated similarly).

## How to Apply It
1. **Audit the Training Data**: Specifically check if your dataset under-represents certain groups or contains historical labels that reflect past prejudices.
2. **Select Fairness Metrics**: Choose the metrics that matter most for your use case (e.g., **Disparate Impact**, **Equal Opportunity**, or **Demographic Parity**).
3. **Perform Segmented Evaluation**: Test your model's performance (Precision/Recall) separately for every major demographic group to identify "performance gaps."
4. **Implement Mitigation Techniques**: Work with ML engineering to apply "Pre-processing" (balancing the data), "In-processing" (adding fairness constraints to the model), or "Post-processing" (adjusting the outputs).
5. **Establish a "Fairness Council"**: Create a cross-functional group (Legal, Ethics, Product, Eng) to review high-stakes AI features before launch.

## Connected Concepts
- [[04 - Data Strategy/Data Quality]] — the primary source of bias in AI systems.
- [[08 - Responsible AI/Transparency to Users]] — the requirement to be honest about model limitations and bias risks.
- [[08 - Responsible AI/Fairness Metrics]] — the specific technical scores used to measure bias.
