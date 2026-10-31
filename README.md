# Vector Databases: From Zero to RAG

A complete, hands-on course that takes you from "what is a vector?" to building and evaluating a production-grade Retrieval-Augmented Generation system. The course is structured in nine sessions across three progressive parts, each pairing a theory lecture with a practical lab.

All labs run on **Google Colab** with **Python** -- no local setup, no GPU, and no paid APIs required.

---

## Table of Contents

- [Who This Course Is For](#who-this-course-is-for)
- [What You Will Learn](#what-you-will-learn)
- [Course Structure](#course-structure)
- [Repository Layout](#repository-layout)
- [Technologies and Tools](#technologies-and-tools)
- [Getting Started](#getting-started)
- [Prerequisites](#prerequisites)
- [License](#license)

---

## Who This Course Is For

- Developers who want to understand vector search and build AI-powered retrieval systems.
- Data scientists and ML engineers exploring RAG architectures.
- Backend engineers evaluating vector databases for their stack.
- Anyone who wants a structured, project-driven path into the vector database ecosystem.

---

## What You Will Learn

- Why traditional keyword search breaks down and how semantic search solves it.
- How text and images become numerical vectors through embeddings.
- The math behind similarity: cosine similarity, dot product, and Euclidean distance.
- How approximate nearest neighbor algorithms (HNSW, IVF, PQ, LSH) make search fast.
- How to choose between FAISS, Qdrant, pgvector, Pinecone, Weaviate, Milvus, and ChromaDB.
- Text chunking strategies and their impact on retrieval quality.
- ChromaDB from installation to advanced queries with metadata filtering.
- Building a full RAG pipeline: retrieve, augment, generate.
- Evaluating retrieval with recall@k and MRR, and improving it with hybrid search and reranking.

---

## Course Structure

The course is divided into three parts that build on each other progressively.

### Part 1 -- Fundamentals

| Session | Topic | Slides | Lab PDF | Notebook |
|---------|-------|--------|---------|----------|
| 1 | Introduction and the Problem with Traditional Search | [Slides](lectures/Session1_Why_Vector_Databases.pptx) | [Lab](labs/Session1_Lab_Keyword_vs_Semantic_Search.pdf) | [Notebook](notebooks/Lab1_Keyword_vs_Semantic_Search.ipynb) |
| 2 | Embeddings | [Slides](lectures/Session2_Embeddings.pptx) | [Lab](labs/Session2_Lab_Embeddings_and_Visualization.pdf) | [Notebook](notebooks/Lab2_Embeddings_and_Visualization.ipynb) |
| 3 | Similarity Metrics | [Slides](lectures/Session3_Similarity_Metrics.pptx) | [Lab](labs/Session3_Lab_NumPy_Search_Engine.pdf) | [Notebook](notebooks/Lab3_NumPy_Search_Engine.ipynb) |

### Part 2 -- How a Vector Database Works Under the Hood

| Session | Topic | Slides | Lab PDF | Notebook |
|---------|-------|--------|---------|----------|
| 4 | ANN Algorithms and Indexing | [Slides](lectures/Session4_ANN_and_Indexing.pptx) | [Lab](labs/Session4_Lab_FAISS_Index_Benchmark.pdf) | [Notebook](notebooks/Lab4_FAISS_Index_Benchmark.ipynb) |
| 5 | The Vector Database Landscape | [Slides](lectures/Session5_Vector_DB_Landscape.pptx) | [Lab](labs/Session5_Lab_FAISS_vs_Qdrant_vs_pgvector.pdf) | [Notebook](notebooks/Lab5_FAISS_vs_Qdrant_vs_pgvector.ipynb) |
| 6 | Data Preparation and Chunking | [Slides](lectures/Session6_Chunking.pptx) | [Lab](labs/Session6_Lab_Chunking_a_Real_PDF.pdf) | [Notebook](notebooks/Lab6_Chunking_a_Real_PDF.ipynb) |

### Part 3 -- ChromaDB and RAG

| Session | Topic | Slides | Lab PDF | Notebook |
|---------|-------|--------|---------|----------|
| 7 | ChromaDB Fundamentals | [Slides](lectures/Session7_ChromaDB_Fundamentals.pptx) | [Lab](labs/Session7_Lab_ChromaDB_Collections_and_Queries.pdf) | [Notebook](notebooks/Lab7_ChromaDB_Collections_and_Queries.ipynb) |
| 8 | RAG with ChromaDB | [Slides](lectures/Session8_RAG_with_ChromaDB.pptx) | [Lab](labs/Session8_Lab_Ask_Your_Files_RAG.pdf) | [Notebook](notebooks/Lab8_Ask_Your_Files_RAG.ipynb) |
| 9 | Production and Evaluation | [Slides](lectures/Session9_Production_and_Evaluation.pptx) | [Lab](labs/Session9_Lab_Evaluate_and_Harden_RAG.pdf) | [Notebook](notebooks/Lab9_Evaluate_and_Harden_RAG.ipynb) |

---

## Repository Layout

```
Vector-Databases/
|-- lectures/          # Slide decks for each session (.pptx)
|-- labs/              # Lab instruction sheets (.pdf)
|-- notebooks/         # Ready-to-run Colab notebooks (.ipynb)
```

Each session has three matching files: a lecture deck, a lab PDF with guided instructions, and a Jupyter notebook with starter code and exercises.

---

## Technologies and Tools

| Category | Tools |
|----------|-------|
| Language | Python |
| Environment | Google Colab |
| Embeddings | Sentence-Transformers, OpenAI API |
| Vector Libraries | FAISS, NumPy |
| Vector Databases | ChromaDB, Qdrant, pgvector |
| LLM (RAG) | Qwen 2.5 (open-weight, free) |
| Reranking | Cross-encoder models |
| Evaluation | Recall@k, MRR |
| Visualization | PCA, t-SNE, Matplotlib |

---

## Getting Started

1. Clone the repository:
   ```bash
   git clone https://github.com/<your-username>/Vector-Databases.git
   ```

2. Open any notebook in Google Colab:
   - Navigate to the `notebooks/` directory.
   - Click on a notebook file, then use the "Open in Colab" button, or upload it directly to [colab.research.google.com](https://colab.research.google.com).

3. Follow along with the matching lecture slides in `lectures/` and lab instructions in `labs/`.

Each notebook installs its own dependencies in the first cell, so there is nothing to configure locally.

---

## Prerequisites

- Basic Python proficiency (functions, loops, lists, dictionaries).
- Familiarity with the command line and Jupyter notebooks.
- A Google account for accessing Google Colab.
- No prior experience with vector databases, embeddings, or machine learning is assumed.

---

## License

This project is released for educational purposes. See the [LICENSE](LICENSE) file for details.
