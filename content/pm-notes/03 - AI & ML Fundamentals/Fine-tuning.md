---
tags: [ai, technical]
type: concept
branch: 03 - AI & ML Fundamentals
related: ["Large Language Models (LLMs)", "Build vs Buy vs Fine-tune", "Data Collection & Labeling"]
created: 2026-05-05
---

# Fine-tuning

## Definition
Fine-tuning is the process of taking a pre-trained foundation model (like GPT-4 or Llama-3) and training it further on a smaller, domain-specific dataset. This "adapts" the model's weights to better handle specialized terminology, specific formats, or niche reasoning tasks that were not well-covered in the original training. While more complex and expensive than prompt engineering or RAG, fine-tuning is necessary when you need a model to follow a very specific style, adhere to complex structural requirements, or handle proprietary information at high scale.

## How to Apply It
1. **Validate with Prompt Engineering First**: Ensure that you cannot achieve the desired result through simpler, cheaper methods like RAG or advanced prompting.
2. **Curate a High-Quality Dataset**: Collect 100 to 1,000+ high-quality "Input/Output" pairs that represent the exact behavior you want to teach.
3. **Select a Base Model**: Choose a pre-trained model that has the right balance of general intelligence and technical efficiency for your task.
4. **Run the Training Process**: Use tools like OpenAI's fine-tuning API or open-source frameworks (like Hugging Face) to train the model.
5. **Evaluate Against a Baseline**: Test the fine-tuned model against the original base model on a "held-out" test set to ensure it has actually improved without "forgetting" general capabilities.

## Connected Concepts
- [[03 - AI & ML Fundamentals/Large Language Models (LLMs)]] — the foundation models that serve as the starting point for fine-tuning.
- [[11 - Technical PM/Build vs Buy vs Fine-tune]] — the strategic framework for deciding if fine-tuning is the right choice.
- [[04 - Data Strategy/Data Collection & Labeling]] — the critical process of building the dataset for fine-tuning.
