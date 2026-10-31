# Vector Databases Course: From Zero to RAG

A proposed 9-session course. Each session includes **theory slides** and a **hands-on PDF lab**.

---

## Part 1: Fundamentals

### Session 1: Introduction and the Problem with Traditional Search

- What a vector database is and why we need one
- Limits of keyword search (SQL `LIKE` and similar)
- Use cases: semantic search, recommendation, RAG, image search
- **Lab:** Compare keyword search with semantic search on a small dataset

### Session 2: Embeddings

- What an embedding is and how text and images are turned into numbers
- Dimensions and choosing a model (Sentence-Transformers, OpenAI, etc.)
- **Lab:** Generate embeddings for sentences and visualize them with PCA / t-SNE

### Session 3: Similarity Metrics

- Cosine similarity, dot product, and Euclidean distance, and when to use each
- Brute-force kNN
- **Lab:** Build a simple search engine with NumPy, with no database

---

## Part 2: How a Vector DB Works Under the Hood

### Session 4: ANN Algorithms and Indexing

- Why kNN is slow on large datasets
- HNSW, IVF, PQ, and LSH, explained simply
- Balancing accuracy (recall), speed, and memory
- **Lab:** Use FAISS to compare Flat, HNSW, and IVF on speed and accuracy

### Session 5: The Vector Database Landscape

- Library vs. database (FAISS vs. Chroma)
- Pinecone, Weaviate, Milvus, Qdrant, pgvector, and Chroma
- Metadata filtering, hybrid search, and scaling
- How to choose the right tool
- **Lab:** Quickly try pgvector or Qdrant for comparison

### Session 6: Data Preparation (Chunking)

- Text splitting strategies (fixed-size, recursive, semantic)
- Chunk size and overlap, and their effect on search quality
- Metadata design
- **Lab:** Split a real PDF into chunks and prepare it for storage

---

## Part 3: ChromaDB

### Session 7: ChromaDB Fundamentals

- Installation and client types (in-memory, persistent, client-server)
- Collections and the `add` / `query` / `get` / `update` / `delete` operations
- Metadata filters with `where` / `where_document`
- Choosing a distance function and embedding functions
- **Lab:** Build a complete collection and run queries with different filters

### Session 8: A RAG Project with ChromaDB

- RAG architecture: retrieve, then augment, then generate
- Connecting Chroma to an LLM
- **Lab:** Build an "Ask Your Files" app (chat with PDFs)

### Session 9: Production and Evaluation

- Measuring retrieval quality (recall@k, MRR)
- Reranking and hybrid search
- Performance, scaling, security, and deployment
- **Lab:** Evaluate and improve the RAG system from the previous session

---

## Notes on the Structure

- Parts 1 and 2 build the foundational understanding, so ChromaDB feels easy by the time you reach it.
- You can merge Sessions 2 and 3 if your audience already has some background, or split Chroma across additional sessions if you want to go deeper.
- Every lab uses Python and Google Colab, so students need no local setup.
