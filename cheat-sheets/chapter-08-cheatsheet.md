## Chapter 8 Cheat Sheet — OCI AI Portfolio (15% of exam)

### The Four Portfolio Layers

| Layer | What It Is | Who Uses It | Skill Required | Infra Managed By |
|---|---|---|---|---|
| OCI AI Services | Pretrained, ready-to-use APIs (Vision, Language, Speech, Document Understanding, Anomaly Detection, Forecasting) | App developers, business teams | None — just call the API | Oracle (fully abstracted, incl. GPUs) |
| OCI Generative AI service | Managed access to foundation LLMs for generation, summarization, chat; supports fine-tuning | Developers wanting LLM features | Low-moderate (prompt design, optional fine-tuning) | Oracle (dedicated AI clusters for fine-tune/hosting) |
| OCI Data Science | Platform to build, train, deploy custom models (notebooks, model catalog, jobs, pipelines) | Data scientists / ML engineers | High — coding, algorithm selection | Customer selects compute/GPU shapes |
| GPU Infrastructure | Underlying compute (GPU shapes) powering training & inference across layers above | Indirectly all layers | N/A | Customer (Data Science) or Oracle (AI Services, Generative AI) |

### Quick Decision Rule
- **"No ML team, just need a result"** → OCI AI Services
- **"Need text generation/summarization/chat with an LLM"** → OCI Generative AI service
- **"Need to build/train a custom model with full control"** → OCI Data Science
- **"Data lives in Oracle DB, want SQL-based ML, no data movement"** → Oracle Machine Learning (in-database ML)

### GPU Infrastructure Role
- Accelerates matrix-heavy operations in deep learning training & inference.
- OCI Data Science: customer explicitly chooses GPU-backed compute shapes for training.
- OCI Generative AI service: GPUs power dedicated AI clusters for fine-tuning and hosting; customer does not manage GPUs directly.
- OCI AI Services: GPU usage is completely invisible to the customer.

### Common Exam Traps
- Confusing OCI AI Services (no training needed) with OCI Data Science (training required) — look for keywords like "no data science team" vs "custom algorithm."
- Assuming in-database ML requires exporting data — it does NOT; that's the whole point (SQL-based, data stays in Oracle Database).
- Thinking OCI Generative AI service and OCI Data Science are the same — Generative AI is specifically for foundation/LLM models; Data Science is general-purpose custom ML.
- Believing customers must manage GPUs for every layer — only true for OCI Data Science; AI Services and Generative AI service abstract this away.

### Memory Trick
**"Ready → Reason → Research → Rig"**
- Ready = AI Services (ready-to-use)
- Reason = Generative AI (reasoning/generating text)
- Research = Data Science (build/research custom models)
- Rig = GPU infrastructure (the rig powering it all)
