---
tags: [technical, strategy]
type: framework
branch: 11 - Technical PM
related: ["Model Selection Criteria", "Fine-tuning", "Cost Metrics"]
created: 2026-07-26
---

# Build vs Buy vs Fine-tune

## Definition
Build vs. Buy vs. Fine-tune is the core strategic framework for AI execution. **Buy** involves using a third-party API (like OpenAI) for a general-purpose model. **Fine-tune** involves taking a base model and training it on proprietary data to specialize it for a narrow task. **Build** involves training a custom model from scratch or self-hosting an open-source model (like Llama) on your own infrastructure. For a PM, this is a trade-off between **Speed-to-Market** (Buy), **Strategic Differentiation** (Fine-tune), and **Control/Privacy** (Build).

## How to Apply It
1. **Start with "Buy" (The Prototype)**: Always validate the user value with an off-the-shelf API first. If users don't love the feature with GPT-4, they won't love it with a custom model either.
2. **Evaluate the "Proprietary Data" Advantage**: If you have unique data that no one else has, **Fine-tuning** is the path to creating a model that outperforms generic competitors.
3. **Analyze the Cost-at-Scale**: If your feature is going viral and your API bill is exploding, "Building" (self-hosting an open-source model) can improve your gross margins by 80-90%.
4. **Consider the "Control" Requirement**: If you need a model to never change and to be fully auditable, you must move away from "Black Box" APIs toward a "Build/Self-host" strategy.
5. **Review Every 6 Months**: Technology moves so fast that a feature that required "Building" last year might be a "Buy" commodity today.

## Connected Concepts
- [[11 - Technical PM/Model Selection Criteria]] — the framework used to pick the specific model after the "Build vs Buy" decision is made.
- [[03 - AI & ML Fundamentals/Fine-tuning]] — the technical process that represents the "middle path" of this framework.
- [[07 - Metrics & Analytics/Cost Metrics]] — the primary business driver for moving from "Buy" to "Build."
