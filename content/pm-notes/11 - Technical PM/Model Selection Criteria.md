---
tags: [technical, strategy]
type: framework
branch: 11 - Technical PM
related: ["Large Language Models (LLMs)", "Inference & Latency", "Cost Metrics"]
created: 2026-07-26
---

# Model Selection Criteria

## Definition
Model Selection Criteria is the framework used by PMs and Engineers to decide which machine learning model to use for a specific feature. In the era of "Foundation Models," this involves choosing between **Closed-source APIs** (e.g., GPT-4, Gemini, Claude) and **Open-source Models** (e.g., Llama-3, Mistral). The selection is a multi-variable trade-off between **Intelligence** (reasoning capability), **Latency** (speed), **Cost** (per token), **Context Window** (memory), and **Data Privacy** (where the data is processed).

## How to Apply It
1. **Benchmark on your "Real" Data**: Don't trust general benchmarks (like MMLU); test 3-5 different models on a "Golden Set" of your actual user prompts and desired outputs.
2. **Define your "Efficiency Frontier"**: Map the models on a chart showing **Cost vs. Quality**. Usually, you want the cheapest model that hits your "Utility Threshold."
3. **Assess Context Window Needs**: If your feature involves summarizing 100-page documents, you must prioritize models with large context windows (100K+ tokens).
4. **Evaluate Data Residency**: If you are in a regulated industry (Finance/Healthcare), "Open-source on your own VPC" might be the only viable choice for privacy.
5. **Plan for "Multi-model" Orchestration**: Use a high-quality model for complex reasoning and a smaller, faster model for simple classification or summarization tasks within the same feature.

## Connected Concepts
- [[03 - AI & ML Fundamentals/Large Language Models (LLMs)]] — the category of technology being selected.
- [[07 - Metrics & Analytics/Cost Metrics]] — the primary business constraint on model selection.
- [[03 - AI & ML Fundamentals/Inference & Latency]] — the primary technical constraint on model selection.
