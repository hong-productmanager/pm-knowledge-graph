---
tags: [data, operations]
type: concept
branch: 04 - Data Strategy
related: ["Data Collection & Labeling", "Bias & Fairness", "Data Pipelines"]
created: 2026-07-26
---

# Data Quality

## Definition
Data Quality is the measure of how well a dataset satisfies the requirements for its intended use in a product or model. In AI, "Garbage In, Garbage Out" is the ultimate rule: the performance ceiling of any model is set by the quality of its training data. Data quality is typically measured across four dimensions: **Completeness** (no missing values), **Consistency** (uniform formats), **Accuracy** (reflecting ground truth), and **Timeliness** (freshness). High-quality data ensures that model predictions are reliable, fair, and actionable.

## How to Apply It
1. **Define Quality Standards**: Establish clear "schemas" and validation rules for all incoming data sources.
2. **Implement Data Profiling**: Regularly run statistical checks to identify outliers, missing values, or unexpected shifts in data distribution.
3. **Audit for Bias**: Specifically check if your data under-represents certain groups or reflects historical prejudices that the model might amplify.
4. **Automate Validation**: Build "Data Quality Checks" into your pipelines that automatically flag or block corrupted data from entering the warehouse.
5. **Establish Data Stewardship**: Assign clear ownership for the health of each major data source, ensuring there is a "point person" for quality issues.

## Connected Concepts
- [[04 - Data Strategy/Data Collection & Labeling]] — the process of creating the "Ground Truth" for quality data.
- [[08 - Responsible AI/Bias & Fairness]] — the ethical dimension of data quality analysis.
- [[04 - Data Strategy/Data Pipelines]] — the infrastructure that must enforce quality standards.
