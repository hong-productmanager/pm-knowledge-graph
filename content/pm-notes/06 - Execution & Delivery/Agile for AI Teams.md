---
tags: [execution, agile, process]
type: framework
branch: 06 - Execution & Delivery
related: ["Technical Debt in AI", "Online vs Offline Evaluation", "Model Drift & Degradation"]
created: 2026-07-26
---

# Agile for AI Teams

## Definition
An adaptation of Agile and Scrum methodologies designed to accommodate the non-linear nature of machine learning development, including research spikes, model training cycles, and the inherent uncertainty of experimental outcomes.

## How to Apply It
1. Use Research Spikes: Dedicate specific time-boxed periods for data exploration and feasibility testing.
2. Decouple Research from Integration: Allow the ML team to iterate on models in parallel with the product team building the UI.
3. Measure Progress by "Learning" as well as "Shipping": Value the data insights gained from a failed model experiment.
4. Implement Model Training Sprints: Recognize that training and evaluation have different cadences than standard front-end development.

## Connected Concepts
- [[06 - Execution & Delivery/Technical Debt in AI]] — is often the result of rushing ML cycles to fit standard Agile sprints
- [[07 - Metrics & Analytics/Online vs Offline Evaluation]] — are the "Checkpoints" used to measure progress in an AI sprint
- [[03 - AI & ML Fundamentals/Model Drift & Degradation]] — is the primary risk that Agile monitoring should mitigate post-launch
