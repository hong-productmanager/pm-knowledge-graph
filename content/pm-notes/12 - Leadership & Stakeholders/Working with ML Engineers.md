---
tags: [leadership, technical]
type: concept
branch: 12 - Leadership & Stakeholders
related: ["PM-Engineering Collaboration", "Managing ML Models as Products", "Model Evaluation (Offline)"]
created: 2026-07-26
---

# Working with ML Engineers

## Definition
Working with ML Engineers refers to the specialized collaboration required to build, deploy, and maintain machine learning models. Unlike traditional software engineering, where logic is "deterministic" (If X, then Y), ML engineering is "probabilistic" and research-intensive. A PM's role is to bridge the gap between "Mathematical Excellence" and "Product Value," ensuring that the engineers are optimizing for the metrics that actually matter to users and the business.

## How to Apply It
1. **Define the "Objective Function" Together**: Ensure you both agree on what the model should be "trying to do" (e.g., maximize clicks vs. maximize long-term retention).
2. **Translate Product Requirements to Technical Constraints**: Instead of saying "make it fast," say "it must have a P99 latency of <200ms to work in our real-time UI."
3. **Respect the "Experimentation Cycle"**: Understand that ML engineers need time for "Training Runs" and "Hyperparameter Tuning" which can't always be perfectly scheduled in a 2-week sprint.
4. **Build a Shared "Golden Set"**: Collaborate on the 1,000 "Perfect Examples" that the model must get right before it can be considered a success.
5. **Ask for "Confidence Intervals"**: Instead of asking "Is it right?", ask "How sure is the model of this result, and what are the known failure modes?"

## Connected Concepts
- [[11 - Technical PM/PM-Engineering Collaboration]] — the broader context of technical partnership.
- [[11 - Technical PM/Managing ML Models as Products]] — the shared goal of this collaboration.
- [[03 - AI & ML Fundamentals/Model Evaluation (Offline)]] — the technical metrics that drive the daily work of ML engineers.
