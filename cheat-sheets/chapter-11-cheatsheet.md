## OCI Generative AI Service & Oracle Database 23ai — Cheat Sheet

### OCI Generative AI: Usage Modes
| Mode | Infrastructure | Use Case | Supports Fine-Tuned Models? |
|---|---|---|
| On-Demand | Shared, multi-tenant | Quick calls to pretrained models, pay-per-call | No |
| Dedicated AI Cluster | Reserved GPU capacity | Fine-tuning and/or hosting custom models | Yes |

### Dedicated AI Cluster Types
| Type | Purpose |
|---|---|
| Fine-Tuning Cluster | Trains a custom model on your data |
| Hosting Cluster | Serves inference for a fine-tuned (or dedicated) model, min. commitment 744 unit-hours |

### Fine-Tuning Methods
| Method | Resource Use | Best For |
|---|---|---|
| T-Few | Low (parameter-efficient) | Small custom datasets, fast iteration |
| Vanilla | High (full fine-tune) | Large custom datasets, deep adaptation |

### Foundation Model Families
- **Cohere**: Command (generation), Embed (embeddings)
- **Meta Llama**: general-purpose chat/generation models
- NOT included: GPT-4, Claude, PaLM (common wrong answers)

### OCI Generative AI Agents
- Managed RAG service: LLM + retrieval over connected data sources
- Supported knowledge sources: Oracle Database 23ai (Vector Search), OCI Object Storage
- No custom retrieval pipeline code required

### Oracle Database 23ai — AI Vector Search
| Feature | Detail |
|---|---|
| Data Type | VECTOR — up to 65,535 dimensions |
| Index Types | HNSW (in-memory graph, fast ANN), IVF (partitioned, disk-based) |
| Distance Metrics | COSINE, DOT, EUCLIDEAN, MANHATTAN |
| Similarity Function | VECTOR_DISTANCE(col, :vec, metric) |
| Key Benefit | Semantic search via SQL alongside existing relational data — no separate vector DB needed |

### Choosing the Right Service
| Need | Use |
|---|---|
| Generate/summarize text via LLM | OCI Generative AI (on-demand or dedicated) |
| Custom-trained model for domain-specific tasks | OCI Generative AI dedicated cluster (fine-tuning + hosting) |
| Conversational Q&A grounded in enterprise docs, no pipeline build | OCI Generative AI Agents (RAG) |
| Store/query embeddings with SQL inside existing Oracle data | Database 23ai AI Vector Search |

### Common Exam Traps
- Confusing **on-demand** (pretrained only) with **dedicated cluster** (required for fine-tuned models)
- Assuming Database 23ai Vector Search is an LLM service — it is NOT; it's vector storage/retrieval
- Assuming Generative AI Agents stores vectors itself — it orchestrates retrieval over external sources like 23ai
- Mixing up T-Few (efficient) vs Vanilla (full) fine-tuning resource profiles
- Picking GPT-4/Claude/PaLM as OCI Generative AI models — only Cohere and Meta Llama are offered
