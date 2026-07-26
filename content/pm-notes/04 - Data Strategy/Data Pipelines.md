---
tags: [data, technical]
type: concept
branch: 04 - Data Strategy
related: ["Data as a Product Asset", "Data Quality", "Model Drift & Degradation"]
created: 2026-07-26
---

# Data Pipelines

## Definition
Data Pipelines are the automated systems that extract data from various sources, transform it into a usable format, and load it into a destination (like a data warehouse, feature store, or model training environment). In ML, pipelines are critical for ensuring that the data used for **Training** is identical in structure and processing to the data used for **Inference** (preventing "Training-Serving Skew"). Modern pipelines often include "Feature Stores" to centralize and version the mathematical inputs used by models across different teams.

## How to Apply It
1. **Map the Data Lineage**: Understand where every piece of data in your model comes from and what transformations happen to it along the way.
2. **Ensure Training-Serving Symmetry**: Work with engineering to guarantee that the code used to process data in the "lab" is the exact same code used in "production."
3. **Implement Feature Versioning**: Use a feature store or versioning system so you can easily "roll back" to a previous data state if a new model fails.
4. **Set Up Data Monitoring**: Create alerts for pipeline "freshness" (is data arriving on time?) and "validity" (is the data format what we expected?).
5. **Optimize for Latency**: For real-time features, ensure the pipeline can process and serve data fast enough to stay within your latency budget.

## Connected Concepts
- [[04 - Data Strategy/Data as a Product Asset]] — the raw material that the pipelines process.
- [[04 - Data Strategy/Data Quality]] — the standards that the pipeline must enforce at every step.
- [[03 - AI & ML Fundamentals/Model Drift & Degradation]] — the problem that pipelines help solve through automated retraining.
