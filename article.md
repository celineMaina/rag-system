# Simple RAG Systems.

You have probably heard the word 'RAG' come up many times in tech circles, and would like to know what it is, how it works and how to implement. In this article, I will explain:

1. What is RAG.
2. Why we use RAG.
3. How RAG works.

### What is RAG?
**RAG** stands for *Retrieval-Augmented Generation*. Let's assume that you are an employee at a tech company. You have been tasked with writing a proposal for a specific project. You would like to use generative AI to help you write.

You may turn to a genAI tool such as Anthropic's Claude. Large Language Models(LLMs) generate original, human-like text according to a user's prompt. Their output is based on generalized, publicly available data, which they are trained on. At best, it would give you a generalized outline for a proposal, which you could not present without customizing, and adding information. There are techniques to improve LLM responses such as fine-tuning which can be expensive and time consuming, and prompt engineering. If you added a copy of your company's guidelines for writing proposals, context about the project and used an effective prompt engineering framework, you will get a better, more tailored response. However, following this process every time you need to use an LLM is not too efficient.

This is where RAG comes in. From the name, we can deduce that it is a framework that enhances/optimizes the output capabilities of an LLM. It does this by first referencing an authorized knowledge base such as internal policy documents, before generating a response. This ensures that the LLM output is up to date and relevant to you. 

### Why RAG is important.
This eliminates the need to retrain or fine-tune models, and reduces model hallucinations.

### How Does RAG work?
