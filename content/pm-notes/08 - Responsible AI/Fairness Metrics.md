---
tags: [responsible-ai, metrics]
type: metric
branch: 08 - Responsible AI
related: ["Bias & Fairness", "Explainability (XAI)", "Model Evaluation (Offline)"]
created: 2026-07-26
---

# Fairness Metrics

## Definition
Fairness Metrics are the quantitative indicators used to measure how equitably an AI system performs across different demographic groups (e.g., race, gender, age). Because "fairness" is a philosophical concept, engineers have developed several mathematical definitions:
1. **Demographic Parity**: Ensuring that the "Positive Prediction Rate" is the same for all groups (e.g., 20% of men and 20% of women are approved).
2. **Equalized Odds**: Ensuring that the "True Positive Rate" and "False Positive Rate" are the same for all groups (e.g., the model is equally likely to correctly identify a qualified candidate regardless of gender).
3. **Individual Fairness**: Ensuring that "similar individuals" receive "similar outcomes."

## How to Apply It
1. **Identify the "Protected Attributes"**: Determine which demographic groups are at risk of being marginalized by your model's decisions.
2. **Select the "Target Definition"**: Choose the metric that best aligns with your ethical and product goals (e.g., "Equal Opportunity" for hiring vs. "Accuracy" for medical triage).
3. **Segmented Evaluation**: Run your offline evaluation separately for each group and compare the scores.

## Connected Concepts
- [[08 - Responsible AI/Bias & Fairness]] — the qualitative problem that these metrics aim to quantify.
- [[03 - AI & ML Fundamentals/Model Evaluation (Offline)]] — the broader technical framework these metrics live within.
- [[08 - Responsible AI/EU AI Act]] — the legal framework that mandates these measurements.
