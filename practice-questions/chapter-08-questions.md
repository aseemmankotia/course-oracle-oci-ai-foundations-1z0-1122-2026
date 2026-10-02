## Chapter 8: Get Started with the OCI AI Portfolio — Practice Questions

**Q1.** A retail company wants to automatically detect the sentiment of thousands of customer reviews per day. They have no data science team and want a solution they can call via a REST API without training any models. Which portfolio layer BEST meets this requirement?

A) OCI Data Science
B) Oracle Machine Learning (in-database ML)
C) OCI AI Services (Language)
D) OCI Generative AI service — fine-tuned custom model

<details>
<summary>Answer</summary>

**Correct: C**

OCI AI Services expose pretrained, ready-to-use capabilities like sentiment analysis through a simple API call — no model building or ML expertise required.

**Why the others are wrong:**
- OCI Data Science requires building, training, and deploying a custom model, which needs data science skills the company lacks.
- In-database ML is meant for building/scoring models on data already in Oracle Database using SQL, not a plug-and-play sentiment API.
- Fine-tuning a Generative AI model adds unnecessary complexity and cost when a pretrained AI Service already solves the problem.

> ⚠️ Frequently missed on the exam — read the options carefully.

</details>

---

**Q2.** A data science team wants full control to write custom Python code, choose their own algorithms, use Jupyter notebooks, and manage the full ML lifecycle including model versioning and deployment pipelines. Which OCI service is designed for this?

A) OCI AI Services
B) OCI Data Science
C) OCI Generative AI service
D) Oracle Machine Learning (in-database ML)

<details>
<summary>Answer</summary>

**Correct: B**

OCI Data Science is the platform layer for building, training, and managing custom models with open-source tools like JupyterLab, model catalogs, jobs, and pipelines.

**Why the others are wrong:**
- OCI AI Services are prebuilt and do not allow custom algorithm development.
- OCI Generative AI service focuses on large language model access, not general custom ML model building.
- In-database ML runs algorithms inside Oracle Database using SQL, not a full custom Python/notebook workflow.

</details>

---

**Q3.** A company stores all its transactional data in Oracle Database and wants to build a fraud-detection model directly on that data without exporting it to another platform, using SQL-based ML functions. Which capability fits this need?

A) OCI Data Science notebooks
B) Oracle Machine Learning (in-database ML)
C) OCI Generative AI service
D) OCI AI Vision service

<details>
<summary>Answer</summary>

**Correct: B**

In-database ML (Oracle Machine Learning) runs ML algorithms directly inside Oracle Database, letting analysts build and score models with SQL without moving data.

**Why the others are wrong:**
- OCI Data Science requires exporting or connecting to data outside the database context for notebook-based development.
- OCI Generative AI service is for LLM-based text tasks, not tabular fraud detection.
- OCI AI Vision is a computer vision service, unrelated to transactional fraud detection.

> ⚠️ Frequently missed on the exam — read the options carefully.

</details>

---

**Q4.** Which OCI service gives applications access to pretrained large language models for tasks such as text generation, summarization, and chat, with the option to customize via fine-tuning?

A) OCI Generative AI service
B) OCI Data Science
C) OCI AI Language
D) Oracle Machine Learning

<details>
<summary>Answer</summary>

**Correct: A**

OCI Generative AI service is the managed layer providing access to foundation LLMs for generative tasks, with fine-tuning support via dedicated AI clusters.

**Why the others are wrong:**
- OCI Data Science is for building custom models generally, not specifically managing foundation LLMs.
- OCI AI Language handles narrower NLP tasks like entity extraction and sentiment, not general-purpose generative text.
- Oracle Machine Learning is in-database ML, unrelated to LLM hosting.

</details>

---

**Q5.** Which layer of the OCI AI portfolio is designed so that customers never need to provision, manage, or scale any GPU infrastructure themselves?

A) OCI Data Science
B) OCI Generative AI service with dedicated AI clusters
C) Custom GPU compute instances
D) OCI AI Services

<details>
<summary>Answer</summary>

**Correct: D**

OCI AI Services fully abstract the underlying infrastructure, including GPUs — customers only call an API and OCI manages all compute behind the scenes.

**Why the others are wrong:**
- OCI Data Science users typically choose and provision compute/GPU shapes for notebooks and jobs.
- Dedicated AI clusters in Generative AI service require the customer to select and pay for reserved GPU-backed capacity for fine-tuning/hosting.
- Custom GPU compute instances are explicitly infrastructure the customer manages directly.

> ⚠️ Frequently missed on the exam — read the options carefully.

</details>

---

**Q6.** A company wants to adapt a foundation model in OCI Generative AI service to better understand their industry-specific terminology using their own labeled dataset. Which approach should they configure?

A) Fine-tune the model on a dedicated AI cluster with their custom dataset
B) Use the base model as-is with prompt engineering only
C) Move the workload to OCI AI Services
D) Train a model from scratch in Oracle Machine Learning

<details>
<summary>Answer</summary>

**Correct: A**

OCI Generative AI service supports fine-tuning foundation models on customer data using a dedicated AI cluster to improve domain-specific accuracy.

**Why the others are wrong:**
- Prompt engineering alone doesn't permanently adapt the model weights to specialized terminology.
- OCI AI Services offer fixed pretrained capabilities and don't support fine-tuning foundation LLMs.
- Oracle Machine Learning is for in-database ML models, not for training/fine-tuning large language models.

> ⚠️ Frequently missed on the exam — read the options carefully.

</details>

---

**Q7.** A team is training a deep learning image classification model with millions of parameters using OCI Data Science. What type of compute shape should they select for efficient training?

A) GPU-accelerated compute shape
B) Standard CPU-only shape
C) Autonomous Database compute shape
D) Object Storage tier

<details>
<summary>Answer</summary>

**Correct: A**

GPU infrastructure accelerates the matrix operations central to deep learning training, making GPU-based shapes the correct choice for large model training in OCI Data Science.

**Why the others are wrong:**
- CPU-only shapes are far slower for deep learning training workloads and not recommended for large models.
- Autonomous Database compute is for database workloads, not model training.
- Object Storage is a storage tier, not a compute resource.

</details>

---

**Q8.** Which statement BEST describes how the four layers of the OCI AI portfolio (AI Services, Generative AI service, Data Science, and underlying GPU infrastructure) relate to each other?

A) They are entirely independent products with no shared infrastructure or lifecycle relationship
B) They form a spectrum from ready-to-use pretrained capabilities to fully custom model development, all powered by shared GPU-based infrastructure
C) Only OCI Data Science uses GPU infrastructure; the other layers run entirely on CPUs
D) AI Services and Generative AI service require customers to manage their own GPU clusters directly

<details>
<summary>Answer</summary>

**Correct: B**

The portfolio spans a lifecycle: AI Services (ready-to-use), Generative AI service (managed LLMs, customizable), and Data Science (fully custom build/train), all underpinned by GPU infrastructure that scales depending on the layer's needs.

**Why the others are wrong:**
- The layers are complementary and often used together across the AI lifecycle, not isolated.
- GPU infrastructure underlies Generative AI and Data Science workloads too, not just Data Science.
- AI Services and Generative AI service abstract infrastructure management away from the customer, contrary to this statement.

> ⚠️ Frequently missed on the exam — read the options carefully.

</details>

---

