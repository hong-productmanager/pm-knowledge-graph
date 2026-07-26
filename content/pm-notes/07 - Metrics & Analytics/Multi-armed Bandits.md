---
tags: [metrics, experimentation]
type: concept
branch: 07 - Metrics & Analytics
related: ["Experimentation", "Online vs Offline Evaluation", "AI Metrics"]
created: 2026-05-05
---

# Multi-armed Bandits

## Definition
Multi-armed Bandits (MAB) is an adaptive experimentation framework that optimizes for a winning variant in real-time, unlike traditional A/B tests that split traffic equally until a fixed conclusion. Named after a gambler at a row of slot machines ("one-armed bandits"), the algorithm balances **Exploration** (trying different versions to find the best) and **Exploitation** (routing more traffic to the current leader). This significantly reduces the "opportunity cost" of showing a suboptimal version to users for the full duration of a test.

## How to Apply It
1. **Identify the Right Use Case**: Choose MAB for features with many variants (e.g., headlines, thumbnails) where you care more about "maximizing the outcome" than "causal proof."
2. **Define the Reward**: Clearly specify what metric the algorithm should optimize for (e.g., clicks, watch time, or conversion).
3. **Set the Exploration Budget**: Determine how much traffic you are willing to "waste" on testing new variants (epsilon-greedy or Thompson sampling).
4. **Integrate with the Product Flow**: Ensure the UI can dynamically switch variants based on the algorithm's real-time decisions.
5. **Monitor for Stability**: Watch for "Feedback Loops" where the algorithm prematurely picks a winner because of a small, early spike in data.

## Connected Concepts
- [[07 - Metrics & Analytics/Experimentation]] — the traditional framework that MAB aims to optimize.
- [[07 - Metrics & Analytics/Online vs Offline Evaluation]] — the process of measuring the real-world "reward" for the bandit.
- [[07 - Metrics & Analytics/AI Metrics]] — the success indicators that the bandit uses as its objective function.
