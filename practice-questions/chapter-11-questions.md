## Chapter 11: OCI Generative AI Service & Oracle Database 23ai — Practice Questions

**Q1.** A company fine-tunes a custom model using OCI Generative AI service and now needs to serve it in production with predictable low-latency inference on dedicated GPU capacity. What must they provision?

A) On-demand inference endpoint only
B) An Autonomous Database instance
C) A dedicated AI cluster (hosting cluster)
D) A standard OCI Compute VM running the model manually

<details>
<summary>Answer</summary>

**Correct: C**

Fine-tuned custom models cannot be served on shared on-demand infrastructure — they require a dedicated AI cluster (hosting type) that reserves GPU capacity exclusively for that model.

**Why the others are wrong:**
- On-demand mode only serves pretrained (out-of-the-box) foundation models, not custom fine-tuned models
- Autonomous Database has no role in hosting or serving a fine-tuned LLM
- Manually running the model on a generic VM bypasses the managed OCI Generative AI service entirely and isn't the supported deployment path

> ⚠️ Frequently missed on the exam — read the options carefully.

</details>

---

**Q2.** An enterprise wants employees to ask natural-language questions and receive answers grounded in internal documents stored in Oracle Database 23ai, without building a custom retrieval pipeline themselves. Which OCI capability BEST fits this need?

A) OCI Generative AI on-demand text generation only
B) OCI Generative AI Agents
C) Oracle Database 23ai Select AI alone
D) OCI Data Science notebook session

<details>
<summary>Answer</summary>

**Correct: B**

OCI Generative AI Agents is the managed service that implements RAG end-to-end, connecting an LLM to enterprise knowledge sources (including Database 23ai) without custom pipeline code.

**Why the others are wrong:**
- Plain on-demand text generation has no retrieval/grounding step, so it can hallucinate instead of using internal documents
- Select AI translates natural language to SQL against relational data; it isn't a RAG/conversational agent over documents
- A Data Science notebook could build a custom RAG pipeline, but that requires custom development, not the managed 'no build' path the question asks for

> ⚠️ Frequently missed on the exam — read the options carefully.

</details>

---

**Q3.** A team already stores product documentation inside Oracle Database 23ai and wants to run semantic similarity search directly with SQL, without exporting data to a separate vector database. Which feature satisfies this?

A) Oracle Database 23ai AI Vector Search (VECTOR data type and vector indexes)
B) OCI Generative AI dedicated cluster
C) OCI Generative AI Agents knowledge base only
D) OCI Object Storage lifecycle rules

<details>
<summary>Answer</summary>

**Correct: A**

23ai introduces the native VECTOR data type plus vector indexes (e.g., HNSW), letting you run similarity search with SQL directly against existing relational data — no separate vector store needed.

**Why the others are wrong:**
- A dedicated AI cluster is for hosting/fine-tuning LLMs, not for storing or searching vectors
- Generative AI Agents can use 23ai as a data source but is a conversational/RAG orchestration layer, not the vector storage capability itself
- Object Storage lifecycle rules manage data tiering/expiry and have nothing to do with vector similarity search

</details>

---

**Q4.** Which foundation model family is available for use within the OCI Generative AI service?

A) OpenAI GPT-4
B) Google PaLM
C) Anthropic Claude
D) Cohere Command

<details>
<summary>Answer</summary>

**Correct: D**

OCI Generative AI service offers Cohere family models (Command, Embed) alongside Meta Llama models as its foundation models.

**Why the others are wrong:**
- GPT-4 is an OpenAI model not offered as a foundation model within OCI Generative AI
- PaLM is a Google model, not part of the OCI Generative AI model catalog
- Claude is an Anthropic model, not part of the OCI Generative AI model catalog

> ⚠️ Frequently missed on the exam — read the options carefully.

</details>

---

**Q5.** A developer needs to quickly call a pretrained foundation model for text summarization, wants to pay only per request, and does not want to manage or reserve any infrastructure. Which OCI Generative AI usage mode should they choose?

A) Dedicated AI cluster (hosting)
B) Dedicated AI cluster (fine-tuning)
C) On-demand mode
D) Custom GPU bare metal instance

<details>
<summary>Answer</summary>

**Correct: C**

On-demand mode uses shared multi-tenant infrastructure with pay-per-call pricing for pretrained models — exactly matching the 'no infrastructure management, pay per request' requirement.

**Why the others are wrong:**
- A hosting cluster reserves dedicated capacity and requires a minimum commitment, which is unnecessary for occasional pretrained-model calls
- A fine-tuning cluster is used to train a custom model, not to serve simple pretrained inference calls
- A bare metal GPU instance requires the developer to manage infrastructure themselves, contradicting the requirement

</details>

---

**Q6.** Which OCI Generative AI fine-tuning method is designed to use fewer compute resources and less training data by updating only a small subset of model parameters?

A) Vanilla (full) fine-tuning
B) Full pretraining from scratch
C) T-Few fine-tuning
D) On-demand prompt engineering

<details>
<summary>Answer</summary>

**Correct: C**

T-Few is the parameter-efficient fine-tuning method in OCI Generative AI, designed to train faster and cheaper on smaller custom datasets by updating only a fraction of model weights.

**Why the others are wrong:**
- Vanilla fine-tuning updates all model weights, requiring significantly more data and compute — the opposite of the scenario
- Pretraining from scratch is not offered in OCI Generative AI's fine-tuning options and is far more resource-intensive
- Prompt engineering doesn't modify model weights at all, so it isn't a fine-tuning method

> ⚠️ Frequently missed on the exam — read the options carefully.

</details>

---

**Q7.** Which vector index organization type in Oracle Database 23ai AI Vector Search provides fast approximate nearest-neighbor search using an in-memory neighbor graph structure?

A) B-tree
B) Bitmap
C) HNSW
D) Reverse key index

<details>
<summary>Answer</summary>

**Correct: C**

HNSW (Hierarchical Navigable Small World) is the in-memory graph-based vector index type in 23ai used for fast approximate nearest-neighbor similarity search.

**Why the others are wrong:**
- B-tree indexes are for scalar column equality/range lookups, not vector similarity
- Bitmap indexes are for low-cardinality columns in analytic queries, unrelated to vectors
- Reverse key indexes address index contention on sequential keys and have no vector search function

</details>

---

**Q8.** What is the primary purpose of the OCI Generative AI Agents service?

A) To store and index vector embeddings inside a relational schema
B) To train new foundation models from raw text corpora
C) To provision and scale GPU clusters for other OCI services
D) To provide a managed retrieval-augmented generation (RAG) conversational experience grounded in enterprise data sources

<details>
<summary>Answer</summary>

**Correct: D**

Generative AI Agents combines a foundation model with retrieval over connected data sources (like Database 23ai or Object Storage) to deliver grounded, conversational answers — the core RAG use case.

**Why the others are wrong:**
- Storing/indexing vector embeddings is the job of Database 23ai AI Vector Search, not the Agents service itself
- Training foundation models from scratch is not something OCI Generative AI Agents or the wider Generative AI service does
- GPU cluster provisioning is handled by dedicated AI clusters, a separate concept from the Agents service

> ⚠️ Frequently missed on the exam — read the options carefully.

</details>

---

