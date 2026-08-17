
# 🤖 Local RAG Knowledge Assistant

A lightweight **Retrieval-Augmented Generation (RAG)** project that combines semantic search with a locally running Large Language Model to generate context-grounded answers.

The project uses **Ollama** to generate text embeddings and LLM responses, **BGE embeddings** to represent knowledge as vectors, **cosine similarity** for semantic retrieval, and **Llama 3.2 1B Instruct** for answer generation.

---

## 📌 Overview

Large Language Models can generate impressive answers, but they may not always have access to specific external information.

This project demonstrates a basic **RAG pipeline** that allows an LLM to answer questions using information retrieved from a custom knowledge base.

Instead of directly asking the LLM a question, the system follows this process:

```text
Knowledge Base
      ↓
Text Processing
      ↓
Embedding Generation
      ↓
Vector Storage
      ↓
User Query
      ↓
Query Embedding
      ↓
Cosine Similarity Search
      ↓
Top Relevant Context
      ↓
Prompt Augmentation
      ↓
Llama 3.2 LLM
      ↓
Context-Grounded Answer
