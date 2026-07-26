---
tags: [ux, ai]
type: pattern
branch: 09 - AI UX Patterns
related: ["Fallback Logic", "Copilot vs Autopilot", "Confidence Indicators"]
created: 2026-05-05
---

# Graceful Degradation

## Definition
Graceful Degradation is a design pattern where an AI product is engineered to remain functional and helpful even when the AI component fails, is uncertain, or is completely unavailable (due to latency, cost, or network issues). Instead of showing a "Loading Error" or a blank state, the product "degrades" to a simpler, more reliable alternative. This involves a **Fallback Hierarchy**:
1. **AI Output** (The ideal state).
2. **Rules-based/Heuristic alternative** (The "safe" state).
3. **Manual path/Human input** (The "legacy" state).

## How to Apply It
1. **Identify the "Critical Path"**: Determine the one thing the user *must* be able to do (e.g., "send a message").
2. **Design the "Safety Net"**: Create a rules-based version of the feature that requires zero AI (e.g., a simple keyword search fallback for a semantic search engine).
3. **Seamless Transitions**: The switch from AI to Fallback should be invisible to the user. No "Loading" spinners or "Error: AI disconnected" banners.
4. **Confidence Thresholds**: Use a "Confidence Indicator" to decide when to trigger the fallback (e.g., if model confidence < 0.6, show the rules-based result instead).

## Connected Concepts
- [[06 - Execution & Delivery/Fallback Logic]] — the technical implementation of this UX pattern.
- [[09 - AI UX Patterns/Copilot vs Autopilot]] — the interaction model that determines how much the user relies on the AI.
- [[09 - AI UX Patterns/Confidence Indicators]] — the signal used to trigger a graceful degradation.
