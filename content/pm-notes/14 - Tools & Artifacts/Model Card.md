---
tags: [artifact, ai]
type: artifact
branch: 14 - Tools & Artifacts
related: ["Red Team Report", "Datasheet for Datasets", "Bias & Fairness"]
created: 2026-05-05
---

# Model Card

## Definition
A Model Card is a standardized, short document providing essential information about a machine learning model. Think of it as a "Nutrition Label" for AI. It typically covers: **Intended Use**, **Out-of-scope uses**, **Training Data description**, **Performance Metrics** across demographic groups, **Known Limitations**, **Ethical Considerations**, and **Contact Information**. Originally proposed by researchers at Google in 2018, it has since become the industry standard for transparent AI documentation.

## How to Apply It
1. **Section 1: Model Details**: Name, version, type, and date.
2. **Section 2: Intended Use**: Who should use it? For what tasks?
3. **Section 3: Factors**: What demographic or environmental factors might affect performance?
4. **Section 4: Metrics**: What were the evaluation scores? (Precision, Recall, F1, etc.)
5. **Section 5: Training & Eval Data**: Where did the data come from? Was it balanced?
6. **Section 6: Quantitative Analysis**: Show the performance "Breakdown" by group to highlight any bias.

## Connected Concepts
- [[14 - Tools & Artifacts/Red Team Report]] — the "Attack" documentation that complements the model card's "Performance" documentation.
- [[14 - Tools & Artifacts/Datasheet for Datasets]] — the documentation for the "Fuel" that created the model.
- [[08 - Responsible AI/Bias & Fairness]] — the core ethical challenge that model cards help to manage.
