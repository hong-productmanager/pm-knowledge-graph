---
tags: [ai, technical]
type: concept
branch: 03 - AI & ML Fundamentals
related: ["RAG (Retrieval Augmented Generation)", "Fine-tuning", "Hallucination"]
created: 2026-05-05
---

# Large Language Models (LLMs)

## Definition
Large Language Models (LLMs) are advanced neural networks trained on massive datasets of text (and sometimes code) to predict the next token in a sequence. They represent a shift in AI from task-specific models to "Foundation Models" that can perform a wide variety of reasoning and creative tasks. Key concepts for PMs include the **Context Window** (the limit on how much text the model can process at once), **Temperature** (controlling the randomness/creativity of the output), and **Prompt Engineering** (the technique of crafting inputs to elicit specific behaviors).

## How to Apply It
1. **Identify the Reasoning Task**: Choose a feature that requires understanding context, summarizing information, or generating content.
2. **Select the Right Model**: Balance performance, cost, and latency (e.g., choosing a "smaller" model for simple tasks vs. a "frontier" model for complex reasoning).
3. **Optimize the Prompt**: Iterate on instructions, using techniques like "Chain of Thought" (asking the model to explain its steps) or "Few-shot" (providing examples).
4. **Manage the Context Window**: Develop strategies for what information to include in the prompt to stay within the model's limits while providing enough context.
5. **Monitor for Hallucination**: Implement safety checks and user UI patterns (like citations) to manage the risk of the model generating false information.

## Connected Concepts
- [[03 - AI & ML Fundamentals/RAG (Retrieval Augmented Generation)]] — the primary way to ground LLMs in current or proprietary data.
- [[03 - AI & ML Fundamentals/Fine-tuning]] — the process of adapting an LLM to a specific domain or style.
- [[03 - AI & ML Fundamentals/Hallucination]] — the core risk associated with the probabilistic nature of LLMs.
