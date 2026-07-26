---
tags: [ux, ai]
type: pattern
branch: 09 - AI UX Patterns
related: ["Copilot vs Autopilot", "User Trust Metrics", "Responsible AI"]
created: 2026-05-05
---

# Human-in-the-Loop UX

## Definition
Human-in-the-Loop (HITL) is a design pattern where a human user is required to review, correct, or approve an AI's output before it is finalized or takes an action in the real world. This is a critical safety and quality mechanism for tasks where model accuracy is not yet 100% or where the "Cost of Failure" is high (e.g., medical diagnosis, financial transfers, or legal filings). HITL transforms the AI from a "solo actor" into a "collaborative assistant" that augment human capabilities rather than replacing them.

## How to Apply It
1. **Identify "High-Stakes" Moments**: Determine the specific actions where an AI error would be catastrophic (e.g., "Send Payment").
2. **Design the "Review" Interface**: Create a UI that highlights the AI's "changes" or "suggestions" clearly, making it easy for the human to spot errors (e.g., Track Changes in Word).
3. **Implement "Approval Queues"**: For autonomous agents, create a dashboard where the human can batch-review and approve several AI tasks at once.
4. **Measure "Human Effort"**: Track how much time the user spends "correcting" the AI; if it takes longer to fix the AI than to do it manually, the HITL pattern is failing.
5. **Gradually Reduce the Loop**: As the model's accuracy improves, move from "Required Approval" to "Optional Review" for lower-risk tasks.

## Connected Concepts
- [[09 - AI UX Patterns/Copilot vs Autopilot]] — how the HITL pattern defines the difference between these two paradigms.
- [[07 - Metrics & Analytics/User Trust Metrics]] — the primary indicator of whether the HITL pattern is working to calibrate user expectations.
- [[08 - Responsible AI/Responsible AI MOC|Responsible AI]] — using HITL as a core ethical guardrail for high-risk systems.
