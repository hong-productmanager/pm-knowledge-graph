---
tags: [ai, operations]
type: concept
branch: 03 - AI & ML Fundamentals
related: ["Feedback Loops", "AI Metrics", "Technical Debt in AI"]
created: 2026-07-26
---

# Model Drift & Degradation

## Definition
**Model Drift** is the phenomenon where a machine learning model's performance decreases over time because the real-world environment it operates in has changed since it was trained. It is generally categorized into **Data Drift** (the distribution of the input data changes) and **Concept Drift** (the relationship between the input and the target output changes). Unlike software bugs, model degradation is "silent" — the system won't crash, but it will start providing lower-quality, less accurate results, leading to a "stealth" loss of product value.

## How to Apply It
1. **Define a Performance Baseline**: Establish the "Golden Set" of data and metrics (e.g., Accuracy, F1) that represents success at launch.
2. **Implement Input Monitoring**: Use statistical tests (like KL Divergence) to detect if the "distribution" of incoming user data is shifting away from the training set.
3. **Track "Proxy" Quality Metrics**: If you cannot get "ground truth" labels quickly, track user behavior (e.g., "acceptance rate" or "override rate") as a leading indicator of drift.
4. **Establish Drift Thresholds**: Set clear alerts for when performance drops below a certain level, triggering an investigation or an automatic retraining pipeline.
5. **Develop a Retraining Strategy**: Decide how often the model needs fresh data — whether it's daily (for news/stock trends) or quarterly (for general language tasks).

## Connected Concepts
- [[04 - Data Strategy/Feedback Loops]] — the systems used to capture new data for retraining after drift is detected.
- [[07 - Metrics & Analytics/AI Metrics]] — the product-level KPIs that often show the first business signs of model degradation.
- [[06 - Execution & Delivery/Technical Debt in AI]] — the long-term cost of ignoring model maintenance and monitoring.
