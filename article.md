# Simple RAG Systems.

You have probably heard the word 'RAG' come up many times in tech circles, and would like to know what it is, how it works and how to implement. In this article, I will explain:

1. What is RAG.
2. Why we use RAG.
3. How RAG works.

### What is RAG?
**RAG** stands for *Retrieval-Augmented Generation*. Let's assume that you are an employee at a tech company. You have been tasked with writing a proposal for a specific project. You would like to use generative AI to help you write.

You may turn to a genAI tool such as Anthropic's Claude. Large Language Models(LLMs) generate original, human-like text according to a user's prompt. Their output is based on generalized, publicly available data, which they are trained on. At best, it would give you a generalized outline for a proposal, which you could not present without customizing, and adding information. 

There are techniques to improve LLM responses such as fine-tuning which can be expensive and time consuming, and prompt engineering. If you added a copy of your company's guidelines for writing proposals, context about the project and used an effective prompt engineering framework, you will get a better, more tailored response. However, following this process every time you need to use an LLM is not too efficient.

This is where RAG comes in. From the name, we can deduce that it is a framework that enhances/optimizes the output capabilities of an LLM. It does this by first referencing an authorized knowledge base such as internal policy documents, before generating a response. This ensures that the LLM output is up to date and relevant to you. 

### Why RAG is important.
Though LLMs are powerful and capable of generating text that is almost indistinguishable from human-written text, their outputs can be unpredictable and inaccurate. LLMs face challenges such as:

- Hallucinations i.e. presenting false information as facts.
- Present outdated information since they rely on static training data with a strict cut-off date.
- May quote false and unverified sources.

RAG is one technique that can be applied to solve these challenges. A RAG system redirects the LLM to refer to an authorized knowledge base before answering a user's query. 

Implementing a RAG system eliminates the need to retrain LLM models with current data all the time, which is very expensive and time-consuming. It ensures that the model remains current, accurate and relevant to your specific context. Additionally, it gives users more control over the generated outputs and the ability to implement guardrails.


### How Does RAG work?
Without RAG, an LLM will provide a response based on its training data, and cannot access and reference domain-specific or proprietary internal documents. With RAG, we introduce retrieval and the LLM must first pull information from a relevant source before generating a response. 

In our scenario, when you prompt the LLM chatbot to help you write a proposal, it will first search the approved knowledge base which may contain your company's guidelines on proposal structure/format, information about the project and other internal documents for reference.

The workflow becomes:

Query → Retrieve relevant documents → Reference the information within the documents → Generate a response.

RAG turns a general-purpose LLM into a domain-specific assistant, enabling it to give precise responses and minimize hallucinations. 