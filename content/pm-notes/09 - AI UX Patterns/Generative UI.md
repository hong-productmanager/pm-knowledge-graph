---
tags: [ux, ai]
type: pattern
branch: 09 - AI UX Patterns
related: ["Large Language Models (LLMs)", "Copilot vs Autopilot", "Transparency to Users"]
created: 2026-05-05
---

# Generative UI

## Definition
Generative UI is a design paradigm where the user interface itself is dynamically created or modified by an AI model in real-time to match the specific intent and context of the user's request. Unlike "Static UI" (pre-defined buttons and menus), Generative UI can "morph" to show a custom dashboard, a specialized chart, or a unique set of controls that only exist for that specific conversation. It represents a shift from "Graphic User Interface" (GUI) to "Language User Interface" (LUI) where the "Chrome" of the app is ephemeral.

## How to Apply It
1. **Define "UI Components" as Tools**: Build a library of small, functional React or HTML components (e.g., "CalendarCard," "PriceChart," "TaskToggle") that the AI can "call."
2. **Implement "Intent Detection"**: Use an LLM to determine when a user's request would be better served by a custom UI rather than just text.
3. **Use "Structured Output"**: Ensure the model returns JSON that specifies which component to render and with what data (using tools like OpenAI's Function Calling).
4. **Design for Transitions**: Ensure that the "morphing" between different UI states is smooth and doesn't confuse the user's mental model of where they are in the app.
5. **Set UI Constraints**: Provide clear "Guardrails" so the AI doesn't generate unusable or broken UI layouts that violate your brand's design system.

## Connected Concepts
- [[03 - AI & ML Fundamentals/Large Language Models (LLMs)]] — the "engine" that interprets intent and selects the UI components.
- [[09 - AI UX Patterns/Copilot vs Autopilot]] — how Generative UI can be used to make both paradigms more effective.
- [[08 - Responsible AI/Transparency to Users]] — disclosing that the interface itself is being influenced by the AI's interpretation of your request.
