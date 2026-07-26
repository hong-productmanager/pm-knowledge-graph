---
tags: [ai, technical]
type: concept
branch: 03 - AI & ML Fundamentals
related: ["Model Evaluation (Offline)", "AI-Specific Prioritization", "Build vs Buy vs Fine-tune"]
created: 2026-05-05
---

# Types of ML Problems

## Definition
Machine Learning problems are categorized based on the nature of the task and the type of data involved. The primary types are: **Classification** (assigning items to discrete categories), **Regression** (predicting a continuous numerical value), **Ranking** (ordering items by relevance), **Clustering** (grouping similar items without labels), **Generation** (creating new content), and **Anomaly Detection** (identifying outliers). Choosing the correct problem type is a foundational PM task, as it dictates the model architecture, data requirements, and evaluation metrics.

## How to Apply It
1. **Define the User Outcome**: Start with the specific value you want to provide (e.g., "help users find the right song").
2. **Analyze the Data Inputs**: What information do you have available? Is it labeled, unlabeled, numerical, or categorical?
3. **Map Outcome to ML Type**:
    - Assigning labels? → **Classification**
    - Predicting a score or price? → **Regression**
    - Ordering a list? → **Ranking**
    - Discovering hidden patterns? → **Clustering**
4. **Select Evaluation Metrics**: Match the metrics to the problem type (e.g., Precision/Recall for classification).
5. **Iterate with Engineering**: Discuss the feasibility and trade-offs of the chosen problem type with your ML engineers.

## Connected Concepts
- [[03 - AI & ML Fundamentals/Model Evaluation (Offline)]] — the metrics used to measure success for each problem type.
- [[05 - Prioritization & Roadmapping/AI-Specific Prioritization]] — deciding which ML problems are worth solving first.
- [[11 - Technical PM/Build vs Buy vs Fine-tune]] — the execution decision once the problem type is identified.
