---
tags: [metrics, ai]
type: concept
branch: 07 - Metrics & Analytics
related: ["Experimentation", "AI Metrics", "Release Management"]
created: 2026-07-26
---

# Online vs Offline Evaluation

## Definition
In AI development, **Offline Evaluation** is the process of testing a model on a "held-out" dataset in a controlled environment before it ever sees a real user. **Online Evaluation** is the measurement of the model's actual impact on user behavior and product metrics after it has been deployed to production. The gap between these two is the "Accuracy-Value Gap." A model can have 95% "offline" accuracy but fail miserably "online" because the real-world data is different or because users react to the AI's output in unexpected ways.

## How to Apply It
1. **Set Baseline Offline Metrics**: Use precision, recall, and F1 on a representative test set to filter out low-quality models early.
2. **Run in "Shadow Mode"**: Deploy the new model to production and let it make "invisible" predictions alongside the live model to compare their outputs on real-world data.
3. **Implement "Champion-Challenger" (A/B) Tests**: Roll out the new model to a small % of users and measure the impact on core product health metrics (e.g., conversion, retention).
4. **Audit the "Gaps"**: If a model performs well offline but poorly online, investigate if the training data is "stale" or if there is a technical skew in the data pipeline.
5. **Iterate the Evaluation Set**: Use the "failures" from online evaluation to update your offline test set, making it more challenging and representative for the next round.

## Connected Concepts
- [[07 - Metrics & Analytics/Experimentation]] — the framework used to conduct online evaluation.
- [[07 - Metrics & Analytics/AI Metrics]] — the specific product indicators measured during online evaluation.
- [[06 - Execution & Delivery/Release Management]] — the specialized process of moving a model from offline to online.
