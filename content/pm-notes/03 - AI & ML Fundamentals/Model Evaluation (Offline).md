---
tags: [ai, metrics]
type: concept
branch: 03 - AI & ML Fundamentals
related: ["AI Metrics", "Online vs Offline Evaluation", "Types of ML Problems"]
created: 2026-07-26
---

# Model Evaluation (Offline)

## Definition
Offline Model Evaluation is the process of testing a machine learning model's performance on a "held-out" dataset before it is deployed to production. This provides a safe, controlled environment to measure how well the model generalizes to new data. Key metrics include **Accuracy** (overall % correct), **Precision** (correctness among positive predictions), **Recall** (ability to find all actual positives), **F1 Score** (a balance of P&R), and **AUC-ROC** (performance across all thresholds). A critical PM task is choosing the right metric based on the "cost of failure" for that specific use case.

## How to Apply It
1. **Define the Success Metric**: Choose the metric that most closely aligns with the user value (e.g., Recall for medical diagnosis, Precision for search ads).
2. **Curate the Test Set**: Ensure the held-out data is diverse and representative of the actual distribution the model will see in the real world.
3. **Analyze the Confusion Matrix**: Look beyond the single accuracy number to see where the model is specifically failing (False Positives vs. False Negatives).
4. **Segment the Evaluation**: Test the model on different sub-groups (e.g., by geography or user type) to identify potential bias or performance gaps.
5. **Set the "Launch Threshold"**: Establish a minimum performance level that must be hit before the model can move to a "Canary" or "Shadow" deployment.

## Connected Concepts
- [[07 - Metrics & Analytics/AI Metrics]] — the product-level metrics that these technical model metrics should drive.
- [[07 - Metrics & Analytics/Online vs Offline Evaluation]] — the critical comparison between "lab" performance and "real-world" performance.
- [[03 - AI & ML Fundamentals/Types of ML Problems]] — how the problem type determines which evaluation metrics are relevant.
