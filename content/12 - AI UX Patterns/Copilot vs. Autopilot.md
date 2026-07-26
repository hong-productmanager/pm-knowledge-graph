---
tags: [ai-ux, copilot, autopilot]
type: concept
branch: AI UX Patterns
related: []
created: 2026-07-26
---

# Copilot vs. Autopilot

## Definition
A design spectrum for how much control an AI feature takes from the user. "Copilot" patterns keep the human in the loop — the AI suggests, drafts, or assists, and a person approves or edits before anything happens. "Autopilot" patterns let the AI act autonomously, ideally with guardrails and an easy undo, without requiring per-action approval.

## Why It Matters for PMs
The right point on this spectrum depends on the cost of a wrong action and the model's reliability for that task — autocomplete-style suggestions tolerate more autonomy than an action that sends money or an email on the user's behalf. Picking autopilot too early (before trust and reliability are earned) is a common cause of AI feature backlash; picking copilot forever caps how much time the feature actually saves.

## How I've Applied It
*(Placeholder — replace with a real example: a feature where you had to decide how much autonomy to grant the AI, and why.)*

## Real-World Example
*(Placeholder — replace with a real example of a product that moved from copilot to autopilot for a specific action, or deliberately stayed copilot.)*

## Connected Concepts
- [[Model Bias & Fairness]]
- [[Retrieval-Augmented Generation (RAG)]]
