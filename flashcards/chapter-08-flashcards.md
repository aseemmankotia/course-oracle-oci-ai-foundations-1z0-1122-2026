## Chapter 8: Get Started with the OCI AI Portfolio — Flashcards

| # | Front (Question) | Back (Answer) |
|---|-----------------|---------------|
| 1 | What is OCI AI Services layer for? | Pretrained, ready-to-use AI capabilities (Vision, Language, Speech, Document Understanding, Anomaly Detection, Forecasting) accessed via API — no ML expertise needed. Exam tip: choose this when the requirement says 'no model training' or 'no data science team.' |
| 2 | What is OCI Data Science platform used for? | Building, training, and deploying custom ML models using open-source tools (JupyterLab notebooks, conda environments, model catalog, jobs, pipelines). Exam tip: choose this when the scenario requires custom algorithms or full ML lifecycle control. |
| 3 | What is in-database ML (Oracle Machine Learning)? | ML algorithms that run directly inside Oracle Database using SQL/AutoML — no data movement required. Exam tip: choose this when data already lives in Oracle Database and must stay there. |
| 4 | What does OCI Generative AI service provide? | Managed access to pretrained large language models (LLMs) for text generation, summarization, and chat, with fine-tuning support on dedicated AI clusters. Exam tip: choose this for LLM/generative text scenarios. |
| 5 | AI Services vs Data Science — who manages the ML model? | AI Services: Oracle manages the pretrained model, customer just calls the API. Data Science: customer builds/trains/manages their own custom model. |
| 6 | Data Science vs In-database ML — where does data need to be? | Data Science: data can be pulled from various sources into notebooks/jobs. In-database ML: data stays inside Oracle Database; models are built/scored with SQL. |
| 7 | Role of GPU infrastructure in the OCI AI lifecycle? | GPUs accelerate training and inference for deep learning and LLM workloads. Used heavily by OCI Data Science (custom training) and Generative AI service (fine-tuning/hosting); AI Services abstract GPU management away entirely from the customer. |
| 8 | Which portfolio layer requires ZERO infrastructure management by the customer? | OCI AI Services — fully managed pretrained APIs; no GPU or compute provisioning needed by the customer. |
| 9 | How does fine-tuning work in OCI Generative AI service? | Customer provides a labeled dataset; fine-tuning runs on a dedicated AI cluster to adapt a foundation model to domain-specific needs, producing a custom model endpoint. |
| 10 | Four OCI AI portfolio layers (top to bottom of abstraction)? | 1) OCI AI Services (ready-to-use), 2) OCI Generative AI service (managed LLMs, customizable), 3) OCI Data Science (build/train custom models), 4) GPU/compute infrastructure underlying all layers. |
| 11 | Scenario: no data team, need object detection in images fast — which layer? | OCI AI Services (Vision) — pretrained, ready-to-use, no custom training required. |
| 12 | Scenario: data scientists need custom deep learning model with GPU-accelerated training and full pipeline control — which layer? | OCI Data Science — provides notebooks, GPU-backed compute shapes, jobs, and pipelines for full custom ML lifecycle. |
