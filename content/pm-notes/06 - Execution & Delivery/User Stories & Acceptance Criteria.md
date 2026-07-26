---
tags: [execution, agile, ai]
type: framework
branch: 06 - Execution & Delivery
related: ["AI PRD", "Graceful Degradation", "Confidence Indicators"]
created: 2026-07-26
---

# User Stories & Acceptance Criteria

## Definition
The process of drafting user stories and acceptance criteria (AC) for AI features, which must include explicit handling of probabilistic outcomes, edge cases for model uncertainty, and specific requirements for fallback behavior.

## How to Apply It
1. Incorporate Confidence Levels: Write stories that specify how the UI should change based on model confidence.
2. Define Fallback Actions: Include AC for what happens when the AI service is down or the result is invalid.
3. Detail Negative Constraints: Specify what the AI must *not* do (e.g., "AI must not provide medical advice").
4. Plan for User Feedback: Include stories for capturing "Thumbs up/down" to feed the model's improvement loop.

## Connected Concepts
- [[06 - Execution & Delivery/AI PRD]] — provides the high-level requirements that these stories break down
- [[09 - AI UX Patterns/Graceful Degradation]] — is the design pattern implemented via these user stories
- [[09 - AI UX Patterns/Confidence Indicators]] — are the UI elements often required by AI acceptance criteria
