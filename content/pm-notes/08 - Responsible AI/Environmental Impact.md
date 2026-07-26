---
tags: [responsible-ai, sustainability]
type: concept
branch: 08 - Responsible AI
related: ["Cost Metrics", "Build vs Buy vs Fine-tune", "Inference & Latency"]
created: 2026-05-05
---

# Environmental Impact of AI

## Definition
The Environmental Impact of AI refers to the ecological footprint of machine learning systems, primarily measured in carbon emissions (CO2e) and water consumption. This impact occurs in two major stages: **Training** (the one-time, massive energy cost to build a model) and **Inference** (the recurring, marginal energy cost every time a user makes a query). While training a large model like GPT-3 can emit ~550 tonnes of CO2, the aggregate cost of inference for millions of daily users can quickly surpass training costs within a year of operation.

## How to Apply It
1. **Model Distillation**: Train a smaller "student" model to replicate the performance of a large "teacher" model for inference.
2. **Quantization**: Reduce the precision of model weights (e.g., from FP32 to INT8) to lower the compute required for each token.
3. **Regional Compute**: Schedule heavy training jobs in data centers powered by 100% renewable energy or during "off-peak" hours when the grid is cleanest.

## Connected Concepts
- [[07 - Metrics & Analytics/Cost Metrics]] — the financial side of the environmental footprint.
- [[11 - Technical PM/Build vs Buy vs Fine-tune]] — the strategic choice that determines your long-term energy consumption.
- [[03 - AI & ML Fundamentals/Inference & Latency]] — the technical performance metrics that drive energy usage.
