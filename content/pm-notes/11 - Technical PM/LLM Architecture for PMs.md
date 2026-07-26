---
tags: [technical, ai]
type: concept
branch: 11 - Technical PM
related: ["Large Language Models (LLMs)", "Inference & Latency", "Model Selection Criteria"]
created: 2026-05-05
---

# LLM Architecture for PMs

## Definition
LLM Architecture for PMs refers to the high-level understanding of how a Large Language Model system is structured, from the user's prompt to the final output. This includes the **Frontend** (UI), the **Orchestration Layer** (managing prompts, memory, and tool use), the **Model Layer** (the LLM itself), and the **Data Layer** (Vector DBs and RAG). For a PM, the "architecture" is less about the internal neural weights and more about how these components interact to deliver speed, accuracy, and cost-efficiency.

## How to Apply It
1. **Map the Request/Response Flow**: Draw a diagram showing how a user's query travels through the retriever, the prompt template, and the model.
2. **Select the Orchestration Framework**: Decide whether to use a library like **LangChain** or **LlamaIndex** to manage the complexity of multi-step AI tasks.
3. **Design the Prompt Pipeline**: Create a system for versioning and testing prompts independently of the model code.
4. **Implement Caching**: Work with engineering to store common AI responses in a cache to reduce latency and cost for frequently asked questions.
5. **Establish Monitoring**: Set up tracing (using tools like LangSmith or Arize) to see exactly where "reasoning" goes wrong in the multi-component architecture.

## Connected Concepts
- [[03 - AI & ML Fundamentals/Large Language Models (LLMs)]] — the core component of the architecture.
- [[03 - AI & ML Fundamentals/Inference & Latency]] — the primary performance metric of the architecture.
- [[11 - Technical PM/Model Selection Criteria]] — the logic used to pick the right components for the architecture.
