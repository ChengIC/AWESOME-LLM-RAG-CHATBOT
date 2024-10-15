# RAG (Retrieval Augmented Generation)

## Introduction
RAG is a technique in which we use a large language model (LLM) to generate a response to a user query. The LLM uses the user query to search for relevant documents in a vector database. The LLM then uses the relevant documents to generate a response to the user query.

## When to use RAG vs Fine-tuning?
- Choose **fine-tuning**: 
  - Customize the structure or tone of style of the response
  - Teach a model very complex instruction

- Choose **RAG**:
  - When you just need the specific information to answer the user query
  - Have limited computational resources
  - Reduce hallucination

The analogy for choosing between RAG and fine-tuning is like long-term memory vs short-term memory. However, they are not mutually exclusive and can be used together.

## Fine-tuning Model + RAG
A typical workflow is to fine-tune a model to understand the complext instructions. Then use RAG to provide the specific knowledge. The benefit is that you can use less tokens in the prompt and have more space for the retrieval context. 

## Best Practices for LLM-RAG
1. Start with prompt engineering and few shot prompting to give the model clear and structured instructions.
2. Establish a baseline for your proposed solution.
3. Start small and focus on optimizing fewer high quality training examples.