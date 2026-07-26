---
tags: [data, growth]
type: concept
branch: 04 - Data Strategy
related: ["Data Collection & Labeling", "Model Drift & Degradation", "Feedback Mechanisms"]
created: 2026-05-05
---

# Feedback Loops

## Definition
A Feedback Loop in AI is a system where the outputs of a model and the subsequent reactions of users are captured and fed back into the training process to improve future versions of the model. A **Positive Feedback Loop** occurs when the model gets better with use, attracting more users and more data (the Data Flywheel). A **Negative Feedback Loop** (or bias loop) occurs when the model reinforces its own errors or biases by only showing users what it thinks they like, creating an "echo chamber."

## How to Apply It
1. **Design the "Correction" UX**: Make it effortless for a user to fix an AI mistake (e.g., editing a generated summary) and ensure that "fix" is captured as a new training label.
2. **Define the Objective Function**: Carefully choose what the loop is optimizing for (e.g., "long-term retention" vs. "short-term clicks") to avoid unintended consequences.
3. **Set Up an Automated Pipeline**: Build the infrastructure to move user corrections from the app database back into the model's fine-tuning set.
4. **Monitor for "Loop Poisoning"**: Implement checks to ensure the feedback isn't being manipulated by bot activity or adversarial users.
5. **Close the Loop with the User**: Show users how their feedback is being used (e.g., "Model updated based on your edits") to encourage more high-quality feedback.

## Connected Concepts
- [[04 - Data Strategy/Data Collection & Labeling]] — the raw signals that the feedback loop depends on.
- [[03 - AI & ML Fundamentals/Model Drift & Degradation]] — how the feedback loop can be used to combat silent model decay.
- [[09 - AI UX Patterns/Feedback Mechanisms]] — the specific UI patterns used to capture user reactions.
