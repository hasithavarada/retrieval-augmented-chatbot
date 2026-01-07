# Retrieval-Augmented Chatbot using FAISS and Transformers

This project implements a Retrieval-Augmented Generation (RAG) chatbot
that answers user questions using context retrieved from a large document
corpus.

## 🔹 Overview
- Document source: Project Gutenberg (Sherlock Holmes)
- Chunked long text into overlapping segments
- Generated semantic embeddings using SentenceTransformers
- Stored embeddings in FAISS vector database
- Retrieved top-k relevant chunks using cosine similarity
- Generated answers using a transformer-based language model
- Evaluated responses using ROUGE metrics

## 🔹 Tech Stack
- Python
- LangChain (Text Splitters)
- SentenceTransformers
- FAISS (Vector Database)
- Hugging Face Transformers
- ROUGE Score

## 🔹 Pipeline
1. Document ingestion & cleaning
2. Text chunking with overlap
3. Embedding generation
4. Vector indexing (FAISS)
5. Semantic retrieval
6. Prompt + context injection
7. Answer generation
8. Evaluation using ROUGE

## 🔹 Example Query
**Question:** How is Sherlock Holmes described?

**Retrieved Context:** Top-5 most relevant chunks using cosine similarity

**Answer:** Generated using transformer model with injected context

## 🔹 Results
- Processed ~1,500 text chunks
- Embedding dimension: 384
- Retrieval latency: < 100 ms
- ROUGE-L F1 score: ~0.43

## 🔹 How to Run
```bash
pip install -r requirements.txt
jupyter notebook
