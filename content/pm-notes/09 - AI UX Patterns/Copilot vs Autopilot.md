---
tags: [ux, ai]
type: pattern
branch: 09 - AI UX Patterns
related: ["AI Agents & Tool Use", "Human-in-the-Loop UX", "Trust & Credibility"]
created: 2026-07-26
---

# Copilot vs Autopilot

## Definition
Copilot vs. Autopilot describes the two primary mental models for AI integration in products. A **Copilot** is an assistant that works alongside the user, requiring constant interaction and validation (e.g., code completion or drafting an email). The user remains in the "driver's seat." An **Autopilot** (or Agent) is a system that takes a high-level goal and executes the task autonomously, often in the background, only checking in for final approval or when it hits an error. The choice between these two significantly impacts user trust, friction, and the required level of model accuracy.

## How to Apply It
1. **Analyze Task Complexity and Risk**: Is the task dangerous if done wrong (Copilot) or just annoying and repetitive (Autopilot)?
2. **Evaluate Model Certainty**: If your model's accuracy is 80%, a Copilot is safer; if it's 99.9%, you can move toward Autopilot.
3. **Design for Interaction**:
    - **Copilot**: Focus on low-friction "acceptance" (e.g., Tab to complete) and easy editing.
    - **Autopilot**: Focus on "Progress Transparency" (showing what the agent is doing) and "Approval Checkpoints."
4. **Identify the "Hand-off" Moments**: Clearly define when the AI should stop and wait for human input (e.g., before spending money or sending a public message).
5. **Iterate Toward Autonomy**: Start as a Copilot to build user trust and gather data, then gradually introduce Autopilot features as the model matures.

## Connected Concepts
- [[03 - AI & ML Fundamentals/AI Agents & Tool Use]] — the technical foundation for Autopilot-style features.
- [[09 - AI UX Patterns/Human-in-the-Loop UX]] — the primary design pattern used to manage the "Copilot" experience.
- [[10 - GTM & Growth/Trust & Credibility]] — how the choice of paradigm influences the user's perception of the product's reliability.
