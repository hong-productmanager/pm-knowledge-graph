---
tags: [metrics, ai]
type: metric
branch: 07 - Metrics & Analytics
related: ["Model Evaluation (Offline)", "User Trust Metrics", "Cost Metrics"]
created: 2026-05-05
---

# AI Metrics

## Definition
AI Metrics are the product-level indicators used to measure the performance, impact, and health of machine learning features. While data scientists focus on "Technical Metrics" (like Precision, Recall, and F1), AI PMs must translate these into **"Business/User Metrics"**. These include: **Automation Rate** (% of tasks handled without human input), **User Acceptance Rate** (% of AI suggestions that are accepted), **Override/Correction Rate** (% of AI outputs that users manually edit), and **Hallucination Rate** (% of outputs flagged as factually incorrect).

## How to Apply It
1. **Select the Primary "Value" Metric**: Identify the one metric that best captures the AI's utility (e.g., "Resolution Rate" for a chatbot).
2. **Instrument User Corrections**: Ensure every "undo," "rewrite," or "delete" of an AI output is captured as a "negative" signal in your metrics.
3. **Track "Confidence Calibration"**: Measure how often the model is "confident" but "wrong," as this is the biggest driver of user distrust.
4. **Monitor Cost vs. Performance**: Track the **Cost Per Inference** alongside quality metrics to ensure the feature remains profitable as it scales.
5. **Segment by Model Version**: Use "Champion-Challenger" metrics to compare the live performance of a new model version against the current production model.

## Connected Concepts
- [[03 - AI & ML Fundamentals/Model Evaluation (Offline)]] — the technical metrics that these product metrics should be built upon.
- [[07 - Metrics & Analytics/User Trust Metrics]] — the psychological impact of AI performance on the user base.
- [[07 - Metrics & Analytics/Cost Metrics]] — the financial side of running high-performance AI features.
