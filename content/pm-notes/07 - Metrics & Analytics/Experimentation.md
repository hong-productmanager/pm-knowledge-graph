---
tags: [metrics, process]
type: concept
branch: 07 - Metrics & Analytics
related: ["Online vs Offline Evaluation", "Multi-armed Bandits", "Product Health Metrics"]
created: 2026-05-05
---

# Experimentation

## Definition
Experimentation is the rigorous process of testing hypotheses about product changes using a controlled framework, most commonly **A/B Testing**. It involves splitting users into a **Control group** (current version) and a **Treatment group** (new version) and measuring the impact on a specific metric. Key concepts include **Statistical Significance** (the probability that the result isn't due to chance), **Minimum Detectable Effect (MDE)**, and the **Novelty Effect** (the temporary spike in engagement that occurs just because a feature is new).

## How to Apply It
1. **Draft a Strong Hypothesis**: "If we [Change X], then [Metric Y] will improve by [Z%], because [Reasoning]."
2. **Determine Sample Size and Duration**: Use power analysis to ensure you have enough users to reach a statistically significant result within a reasonable timeframe.
3. **Randomize the Split**: Ensure users are assigned to groups in a way that avoids bias (e.g., don't put all "power users" in the treatment group).
4. **Monitor "Guardrail Metrics"**: Track secondary metrics (like latency or support tickets) to ensure your improvement in one area isn't causing a catastrophic failure in another.
5. **Decide Based on Data, Not Just P-values**: Consider the business context — even if a result is significant, is the improvement large enough to justify the ongoing maintenance cost?

## Connected Concepts
- [[07 - Metrics & Analytics/Online vs Offline Evaluation]] — the comparison between "test" results and real-world production performance.
- [[07 - Metrics & Analytics/Multi-armed Bandits]] — an advanced form of experimentation that optimizes for the "winner" in real-time.
- [[07 - Metrics & Analytics/Product Health Metrics]] — the high-level KPIs that experiments are designed to move.
