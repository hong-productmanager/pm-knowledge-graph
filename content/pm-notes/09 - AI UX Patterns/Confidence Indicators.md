---
tags: [ux, ai]
type: pattern
branch: 09 - AI UX Patterns
related: ["Transparency to Users", "User Trust Metrics", "Hallucination"]
created: 2026-05-05
---

# Confidence Indicators

## Definition
Confidence Indicators are UI elements used to signal how certain an AI model is about a particular prediction, generation, or action. Because AI is probabilistic, it is never "100% sure," but it can provide a "confidence score" for its outputs. These indicators can be **Explicit** (e.g., a percentage score, a "High/Medium/Low" label, or color-coded text) or **Implicit** (e.g., presenting a single answer vs. a list of options). Their primary goal is to help users calibrate their own level of verification effort.

## How to Apply It
1. **Extract Confidence Scores**: Work with engineering to ensure the model's "Logits" or internal probability scores are exposed to the frontend.
2. **Map Scores to User Categories**: Group technical scores (e.g., 0.1 to 1.0) into user-friendly buckets like "Confident" (>0.9) and "Needs Review" (<0.7).
3. **Design the Visual Signal**: Use subtle UI patterns like dimmed text for uncertain words, a "warning" icon for low-confidence summaries, or a "Top 3" list when the model can't pick a winner.
4. **Link to Verification**: If an output is low-confidence, provide an immediate "Verify" button that shows the source data or triggers a secondary check.
5. **Avoid "False Precision"**: Don't show a user "87.42% confident" — it looks technical but provides no more actual utility than "Highly Confident."

## Connected Concepts
- [[08 - Responsible AI/Transparency to Users]] — the broader practice of disclosing AI's probabilistic nature.
- [[07 - Metrics & Analytics/User Trust Metrics]] — the primary success metric that confidence indicators are designed to influence.
- [[03 - AI & ML Fundamentals/Hallucination]] — the risk that confidence indicators help mitigate by signaling uncertainty.
