---
tags: [execution, risk, ux]
type: pattern
branch: 06 - Execution & Delivery
related: ["Graceful Degradation", "Release Management", "Hallucination"]
created: 2026-05-05
---

# Fallback Logic

## Definition
The hierarchy of degradation designed to handle model failures, high latency, or uncertainty. A robust fallback system ensures that the user is always provided with value, moving from the most complex AI solution to a simpler "Rules-based" system, and finally to a manual or "Standard" state.

## How to Apply It
1. Define Confidence Thresholds: Set the level below which the AI output is considered "Unreliable."
2. Implement Heuristic Fallbacks: If the AI fails, use a simple set of "If-Then" rules to provide a baseline answer.
3. Provide Manual Overrides: Allow the user to "Fix" or "Ignore" the AI's mistake easily.
4. Design the "Quiet Failure": In many cases, if the AI is unsure, the best UX is to show nothing at all rather than a broken interface.

## Connected Concepts
- [[09 - AI UX Patterns/Graceful Degradation]] — is the broader design principle that fallback logic enables
- [[06 - Execution & Delivery/Release Management]] — uses fallback logic as a safety net during model rollouts
- [[03 - AI & ML Fundamentals/Hallucination]] — is the specific type of AI error that fallback logic aims to hide or mitigate
