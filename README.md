# Full RAG Pipeline Project

🚀 **Project:** Retrieval-Augmented Generation (RAG) Pipeline  

---

## Overview

This project implements a **full RAG pipeline** from scratch using Python. The pipeline combines:

1. **Retriever (MiniLM)** – performs semantic search to find the most relevant document from a knowledge base.  
2. **Generator (DistilBERT)** – extracts precise answers from the retrieved document.

The pipeline is capable of answering questions based on a custom knowledge base, demonstrating an end-to-end Retrieval-Augmented Generation system.

---

## Features

- Encode a knowledge base into embeddings using **MiniLM**.
- Retrieve the most relevant document for a given query.
- Generate a precise answer using **DistilBERT**.
- Full RAG pipeline function: `ask_rag_pipeline(query)` returning the **answer** and the **retrieved context**.
- CPU/GPU split to optimize resource usage (Retriever on CPU, Generator on GPU if available).

---

## Requirements

```bash
pip install sentence-transformers transformers torch
