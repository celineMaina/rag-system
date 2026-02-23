# Implementing a Simple RAG System.

## Practical Example of Adding RAG to an LLM.

### Background
(Describe a scenario/example where we want to use RAG. This example will be followed and referenced in the code demo)




In the previous article, I gave an overview of a simple RAG system. In this article, I will explain the technical aspects of how RAG works, and provide examples in Python code. 

First, an in-depth, more technical explanation of how RAG works.

### How Does RAG Work?
A simple RAG system connects an LLM to external data sources such as policy documents and company databases, allowing it to answer user questions with relevant, up-to-date information. It works by embedding the reference documents, searching the documents for semantic relevance to the query, then using the retrieved documents to answer the query. 

<figure>
  <img src="RAG-Applications.webp" alt="Simplified RAG Pipeline">
  <figcaption>Photo by <a href="https://writer.com/wp-content/uploads/2023/11/01-RAG-processs-1.png?resize=768,267"></a></figcaption>
</figure>


