---
tags: [ux, ai]
type: pattern
branch: 09 - AI UX Patterns
related: ["Feedback Loops", "Data Collection & Labeling", "User Trust Metrics"]
created: 2026-07-26
---

# Feedback Mechanisms

## Definition
Feedback Mechanisms are UI components that allow users to provide evaluations of an AI's output. This feedback serves two purposes: **Immediate Personalization** (e.g., "Don't show me this again") and **Long-term Model Improvement** (feeding the Data Flywheel). Feedback can be **Binary** (thumbs up/down), **Categorical** (selecting a reason like "too long" or "inaccurate"), or **Free-form** (comments). A successful mechanism must be low-friction while capturing enough context for a data scientist to understand *why* the user was unhappy.

## How to Apply It
1. **Use "Implicit" Feedback First**: Track "Undo," "Delete," and "Regenerate" actions as "Negative Feedback" without the user needing to click a specific thumbs-down button.
2. **Place Mechanisms Near the Output**: Put the thumbs up/down icons immediately following the AI's response so the feedback is "context-aware."
3. **Ask "Why" on Negative Feedback**: If a user clicks "thumbs down," show a quick 2-click menu with options like "Factually Incorrect," "Offensive," or "Too Wordy."
4. **Incentivize High-Quality Feedback**: Show the user that their feedback matters (e.g., "Thanks! We'll use this to improve your future results").
5. **Avoid "Button Fatigue"**: Don't ask for feedback on every single interaction; focus on the high-value or high-uncertainty moments.

## Connected Concepts
- [[04 - Data Strategy/Feedback Loops]] — the technical pipeline that moves the UI feedback into the model's training set.
- [[04 - Data Strategy/Data Collection & Labeling]] — the process of turning user feedback into "Ground Truth" labels.
- [[07 - Metrics & Analytics/User Trust Metrics]] — how the ability to give feedback influences the user's perception of product reliability.
