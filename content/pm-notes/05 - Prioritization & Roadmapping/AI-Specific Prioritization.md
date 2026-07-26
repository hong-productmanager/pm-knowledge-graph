---
tags: [prioritization, ai]
type: concept
branch: 05 - Prioritization & Roadmapping
related: ["Trade-off Frameworks", "Build vs Buy vs Fine-tune", "Model Evaluation (Offline)"]
created: 2026-07-26
---

# AI-Specific Prioritization

## Definition
AI-Specific Prioritization is the practice of adding AI-specific variables to traditional prioritization frameworks. Because AI features are probabilistic and research-heavy, PMs must evaluate factors like **Feasibility** (do we have the data?), **Accuracy Thresholds** (what's the minimum performance needed to be useful?), and **Cold Start Risks** (how much data is needed before the feature works?). It also involves the "Build vs. Buy vs. Fine-tune" decision, as the path chosen significantly impacts the timeline and resource requirements.

## How to Apply It
1. **Assess Data Availability**: For every feature idea, ask: "Do we already have the data, or will we need to spend months collecting and labeling it?"
2. **Define the "Utility Threshold"**: Determine the minimum accuracy or performance level below which the feature provides zero or negative value to the user.
3. **Evaluate the "Cost of Failure"**: Prioritize low-risk AI features (e.g., recommendations) over high-risk ones (e.g., medical advice) if accuracy is still uncertain.
4. **Factor in "Human-in-the-loop" Requirements**: Consider if a feature will require expensive manual review, which adds ongoing operational costs.
5. **Use "Research Spikes"**: Prioritize 1-2 week engineering "spikes" to test feasibility before committing a full quarter to an AI initiative.

## Connected Concepts
- [[05 - Prioritization & Roadmapping/Trade-off Frameworks]] — the general logic used to compare AI and non-AI initiatives.
- [[11 - Technical PM/Build vs Buy vs Fine-tune]] — the execution decision that must be prioritized based on cost and time.
- [[03 - AI & ML Fundamentals/Model Evaluation (Offline)]] — the technical metrics that define whether an AI feature has hit its priority threshold.
