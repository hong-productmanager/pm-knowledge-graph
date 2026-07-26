---
tags: [ux, ai]
type: pattern
branch: 09 - AI UX Patterns
related: ["Confidence Indicators", "Transparency to Users", "Hallucination"]
created: 2026-05-05
---

# Reasoning Disclosure

## Definition
Reasoning Disclosure is an AI UX pattern where the system explains the "why" and "how" behind its output to the user. This spectrum ranges from a **"Black Box"** (no explanation) to a **"Full Chain-of-Thought"** (showing every intermediate step). The goal is to provide just enough disclosure for the user to either **Trust** the answer (if it’s correct) or **Correct** the answer (if it’s wrong), without overwhelming them with technical jargon or excessive detail.

## How to Apply It
1. **Match Disclosure to Stakes**: For high-stakes decisions (e.g., medical or financial), show the full reasoning. For low-stakes (e.g., a music recommendation), keep it hidden.
2. **Source Citations**: Provide inline links to the "Ground Truth" data the AI used. This is the most effective form of disclosure.
3. **Progressive Disclosure**: Show a "summary" of the reasoning by default, with a "Show Details" button for power users.
4. **"Thought Traces"**: Use a "Thinking..." state that shows high-level steps (e.g., "Searching documentation," "Summarizing results," "Checking for bias").

## Connected Concepts
- [[09 - AI UX Patterns/Confidence Indicators]] — signaling "how sure" the AI is, which is a key part of disclosure.
- [[08 - Responsible AI/Transparency to Users]] — the ethical requirement that drives the need for disclosure.
- [[03 - AI & ML Fundamentals/Hallucination]] — the primary failure mode that disclosure helps to mitigate.
