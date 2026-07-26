---
tags: [artifact, ai]
type: artifact
branch: 14 - Tools & Artifacts
related: ["Model Card", "Data Quality", "Data Collection & Labeling"]
created: 2026-05-05
---

# Datasheet for Datasets

## Definition
A Datasheet for Datasets is a standardized document that records the creation, composition, and intended use of a machine learning dataset. If a "Model Card" is a nutrition label for a model, a "Datasheet" is a detailed origin story for the data itself. It covers: **Motivation** (why was it collected?), **Composition** (what’s in it?), **Collection Process**, **Preprocessing** applied, **Intended Uses**, **Distribution Terms**, and a **Maintenance Plan**.

## How to Apply It
1. **Section 1: Motivation**: Who funded the collection? What was the goal?
2. **Section 2: Composition**: How many instances? What are the labels? Are there missing values?
3. **Section 3: Collection**: How was the data acquired? (Scraping, manual labeling, sensor data?)
4. **Section 4: Preprocessing**: Was it cleaned, normalized, or anonymized?
5. **Section 5: Uses**: What tasks is this dataset *not* suitable for? (e.g., "Do not use this for medical diagnosis").
6. **Section 6: Distribution**: How is it shared? What are the license terms?

## Connected Concepts
- [[14 - Tools & Artifacts/Model Card]] — the downstream artifact that relies on the accuracy of the datasheet.
- [[04 - Data Strategy/Data Quality]] — the primary technical metric that datasheets aim to protect.
- [[04 - Data Strategy/Data Collection & Labeling]] — the process that must be documented in the datasheet.
