## Chapter 11: OCI Generative AI Service & Oracle Database 23ai — Flashcards

| # | Front (Question) | Back (Answer) |
|---|-----------------|---------------|
| 1 | OCI Generative AI: minimum commitment period for a dedicated hosting AI cluster? | 744 unit-hours (~31 days). Exam tip: dedicated clusters require a minimum commitment — on-demand mode has no such commitment. |
| 2 | Oracle Database 23ai VECTOR data type — max number of dimensions supported? | Up to 65,535 dimensions. Exam tip: this is the ceiling tested for embedding vector size in 23ai. |
| 3 | OCI Generative AI: on-demand mode vs dedicated AI cluster — key difference? | On-demand = shared infra, pay-per-call, pretrained models only. Dedicated cluster = reserved GPU capacity, required for fine-tuned model hosting or fine-tuning jobs. |
| 4 | OCI Generative AI service vs Oracle Database 23ai AI Vector Search — when to pick which? | Pick OCI Generative AI for LLM inference, chat, summarization, and RAG orchestration (Agents). Pick 23ai AI Vector Search when you need to store/query embeddings with SQL alongside existing relational data. |
| 5 | What are the two types of OCI Generative AI dedicated AI clusters? | Fine-tuning cluster (trains a custom model) and Hosting cluster (serves inference for a fine-tuned or dedicated model). Exam tip: don't confuse the two — fine-tuning trains, hosting serves. |
| 6 | Typical RAG architecture pattern on OCI? | Foundation model (OCI Generative AI) + vector store (Database 23ai AI Vector Search or OCI OpenSearch) + orchestration via OCI Generative AI Agents to ground responses in enterprise data. |
| 7 | SQL function in Oracle 23ai used to compute similarity between vectors? | VECTOR_DISTANCE(col, :vector, COSINE\|DOT\|EUCLIDEAN\|MANHATTAN). Exam tip: know that multiple distance metrics are supported, and COSINE is common for semantic similarity. |
| 8 | Oracle 23ai vector index type used for fast approximate nearest-neighbor search? | HNSW (in-memory neighbor graph). Alternative: IVF (Inverted File Flat, disk-based/partitioned). Exam tip: HNSW = in-memory graph, IVF = partition-based. |
| 9 | Distance metrics supported by Oracle 23ai AI Vector Search? | COSINE, DOT (dot product), EUCLIDEAN, MANHATTAN. Exam tip: cosine is the default choice for semantic/embedding similarity. |
| 10 | OCI Generative AI fine-tuning: T-Few vs Vanilla — when to use each? | T-Few: parameter-efficient, fast, cheaper, good for smaller custom datasets. Vanilla: full fine-tuning of all parameters, needed for large custom datasets requiring deeper adaptation. |
| 11 | Foundation model families available in OCI Generative AI service? | Cohere family (Command, Embed) and Meta Llama family. Exam tip: GPT-4, Claude, and PaLM are NOT OCI Generative AI foundation models. |
| 12 | What data sources can OCI Generative AI Agents ground responses on? | Oracle Database 23ai (AI Vector Search) and OCI Object Storage are supported knowledge base data sources for RAG. Exam tip: Agents = orchestration layer over these sources, not the storage itself. |
