---
tags: [responsible-ai, safety]
type: concept
branch: 08 - Responsible AI
related: ["Transparency to Users", "Hallucination", "Red Team Report"]
created: 2026-07-26
---

# AI Safety & Guardrails

## Definition
AI Safety & Guardrails refer to the layered defense mechanisms and architectural constraints designed to prevent AI systems from producing harmful, biased, or illegal outputs. This is a multi-stage approach that includes **Training-time interventions** (like RLHF and Constitutional AI), **Inference-time filters** (content classifiers that scan prompts and responses), and **Product-level guardrails** (hard blocks, soft warnings, and human review queues). No single layer is sufficient on its own; a robust system requires "Defense in Depth" to handle creative adversarial attacks and unexpected model failures.

## How to Apply It
The "Swiss Cheese" model of safety involves three primary layers:
1. **Model Layer**: Baking principles into the weights (e.g., Anthropic’s Constitutional AI).
2. **Filter Layer**: Using "Safety Classifiers" to intercept and block toxic input or output in milliseconds.
3. **UI/UX Layer**: Implementing "System Prompts" that instruct the model on how to refuse and designing UI that allows for easy reporting.

## Connected Concepts
- [[08 - Responsible AI/Transparency to Users]] — disclosing the existence and purpose of guardrails.
- [[03 - AI & ML Fundamentals/Hallucination]] — how safety filters can also catch factual errors.
- [[14 - Tools & Artifacts/Red Team Report]] — the artifact that proves the effectiveness of your guardrails.
