---
tags: [metrics, ai]
type: metric
branch: 07 - Metrics & Analytics
related: ["AI Metrics", "Confidence Indicators", "Human-in-the-Loop UX"]
created: 2026-05-05
---

# User Trust Metrics

## Definition
User Trust Metrics are a specialized set of indicators used to measure how much users rely on and believe in a product's AI outputs. Unlike general satisfaction, trust is specifically about the **Calibration** between a user's expectations and the model's actual performance. Key metrics include **Override Rate** (how often users manually change an AI output), **Abandonment Rate** (how often users give up on the AI and switch to manual), and **Trust Score** (qualitative measure of reliability). A critical goal is to avoid "Over-trust" (users following the AI when it's wrong) and "Under-trust" (users ignoring the AI even when it's right).

## How to Apply It
1. **Measure the "Silent Rejection"**: Track how often users see an AI suggestion but choose to type their own response instead.
2. **Analyze "Correction Depth"**: Are users making small "style" edits to AI output (High Trust), or are they deleting the entire thing and starting over (Low Trust)?
3. **Perform "Trust Calibration" Surveys**: Ask users "How often do you verify the AI's answer?" to see if their trust level matches the model's actual accuracy.
4. **Monitor "Escalation Rate"**: In chatbots or agents, track how quickly a user asks for a "human," which is a direct proxy for loss of trust in the AI's capability.
5. **Segment Trust by Task Type**: Identify if users trust the AI for "creative" tasks (low stakes) but distrust it for "factual" tasks (high stakes).

## Connected Concepts
- [[07 - Metrics & Analytics/AI Metrics]] — the technical and business metrics that drive the baseline for trust.
- [[09 - AI UX Patterns/Confidence Indicators]] — the UI tools used to manage and calibrate user trust in real-time.
- [[09 - AI UX Patterns/Human-in-the-Loop UX]] — the design pattern that uses human review to protect and build trust.
