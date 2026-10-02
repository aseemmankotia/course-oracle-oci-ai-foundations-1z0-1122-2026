## Chapter 12: Full Exam Simulation & Test-Taking Strategy — Practice Questions

**Q1.** A company wants to extract key-value pairs and tables from scanned mortgage documents, including tables that span multiple pages. Which OCI AI service BEST meets this requirement?

A) OCI Vision
B) OCI Language
C) OCI Speech
D) OCI Document Understanding

<details>
<summary>Answer</summary>

**Correct: D**

Document Understanding is purpose-built to extract key-value pairs, tables, and structured layout data from forms and scanned documents.

**Why the others are wrong:**
- Vision handles image classification, object detection, and basic OCR text extraction, but not structured key-value/table extraction from forms.
- Language performs NLP tasks like entity/sentiment extraction on plain text, not document layout parsing.
- Speech transcribes/translates audio and has nothing to do with document images.

> ⚠️ Frequently missed on the exam — read the options carefully.

</details>

---

**Q2.** A team wants to detect unusual patterns in streaming sensor data from manufacturing equipment to predict failures before they occur. Which OCI AI service is the BEST fit?

A) OCI Anomaly Detection
B) OCI Forecasting
C) OCI Language
D) OCI Vision

<details>
<summary>Answer</summary>

**Correct: A**

Anomaly Detection is designed to flag unusual data points/patterns in time-series or sensor data, ideal for predictive maintenance.

**Why the others are wrong:**
- Forecasting projects continuous future values (e.g., demand, sales) rather than flagging anomalous behavior.
- Language is a text-processing service and does not apply to sensor time-series data.
- Vision processes image/video data, not numeric sensor streams.

> ⚠️ Frequently missed on the exam — read the options carefully.

</details>

---

**Q3.** When customizing a large language model for a narrow, specialized vocabulary (e.g., legal contract clauses) using a small, high-quality labeled dataset, which approach is the BEST choice on OCI Generative AI Service?

A) Fine-tuning
B) Prompt engineering only
C) Increasing the temperature parameter
D) Switching to an embedding model

<details>
<summary>Answer</summary>

**Correct: A**

Fine-tuning adapts model weights using labeled domain data, producing more consistent and reliable output for specialized vocabulary than prompting alone.

**Why the others are wrong:**
- Prompt engineering can help but is less reliable than fine-tuning when a quality labeled dataset exists for a narrow domain — the exam treats fine-tuning as the stronger answer in this scenario.
- Temperature controls output randomness/creativity, not domain adaptation.
- Embedding models are used for semantic search/similarity, not for generating domain-specific text.

> ⚠️ Frequently missed on the exam — read the options carefully.

</details>

---

**Q4.** Which statement BEST differentiates supervised learning from unsupervised learning?

A) Supervised learning only works with images; unsupervised learning only works with text.
B) Supervised learning uses labeled data with known outcomes; unsupervised learning finds patterns in unlabeled data.
C) Supervised learning requires GPUs; unsupervised learning does not.
D) Supervised learning is always more accurate than unsupervised learning.

<details>
<summary>Answer</summary>

**Correct: B**

This is the standard, textbook-accurate distinction tested across AI foundations content.

**Why the others are wrong:**
- Data modality (image vs. text) is unrelated to the supervised/unsupervised distinction.
- Hardware requirements are not a defining characteristic of either learning type.
- Accuracy depends on the problem and data, not the learning paradigm itself.

</details>

---

**Q5.** A data scientist has trained a model in OCI Data Science and needs to expose it as a REST endpoint that scales with request volume for real-time inference. What should they use?

A) OCI Data Science Job
B) OCI Data Science Notebook Session
C) OCI Object Storage
D) OCI Data Science Model Deployment

<details>
<summary>Answer</summary>

**Correct: D**

Model Deployment creates a managed, scalable REST endpoint specifically for serving real-time inference.

**Why the others are wrong:**
- Jobs execute batch or scheduled scripts and do not expose a persistent inference endpoint.
- Notebook Sessions are for interactive development/experimentation, not production serving.
- Object Storage stores artifacts/files; it does not serve model inference requests.

> ⚠️ Frequently missed on the exam — read the options carefully.

</details>

---

**Q6.** During the exam, you encounter a question with unfamiliar terminology, and answering it correctly would require more than a minute of thought. Given the fixed time window and question count, what is the BEST approach?

A) Spend as long as needed since accuracy matters most
B) Skip immediately without selecting any answer and return later if time allows
C) Guess randomly and never revisit it
D) Flag the question, select your best-guess answer now, and move on

<details>
<summary>Answer</summary>

**Correct: D**

Flagging with a best-guess answer locks in a possible correct choice and protects against running out of time before returning, while still allowing reconsideration later.

**Why the others are wrong:**
- Dwelling too long risks not reaching easier questions later in the fixed window.
- Leaving it blank risks forgetting to return, losing a guessable point unnecessarily.
- Never revisiting forfeits the chance that a later question jogs your memory on the same concept.

> ⚠️ Frequently missed on the exam — read the options carefully.

</details>

---

**Q7.** An enterprise wants to build a chatbot that answers employee questions by retrieving relevant passages from internal HR policy documents before generating a response. Which OCI capability combination BEST supports this pattern?

A) OCI Language sentiment analysis alone
B) OCI Vision with object detection
C) OCI Anomaly Detection with a threshold alert
D) OCI Generative AI Agents with a knowledge base (RAG pattern)

<details>
<summary>Answer</summary>

**Correct: D**

Generative AI Agents paired with a knowledge base implement Retrieval-Augmented Generation: retrieve relevant document passages, then generate a grounded answer.

**Why the others are wrong:**
- Sentiment analysis classifies tone/opinion; it does not retrieve documents or generate answers.
- Object detection processes images, irrelevant to text-based document Q&A.
- Anomaly Detection flags unusual data points and has no role in conversational Q&A.

> ⚠️ Frequently missed on the exam — read the options carefully.

</details>

---

**Q8.** You are given a question with four options and can confidently eliminate two as factually incorrect. Of the remaining two, both sound plausible. What is the BEST elimination strategy to apply next?

A) Choose the option that most directly and completely addresses every constraint stated in the question
B) Choose the option that is longest, since detailed answers are usually correct
C) Choose the first of the two remaining alphabetically
D) Choose the option that matches a term you saw earlier in a different question

<details>
<summary>Answer</summary>

**Correct: A**

Re-reading the question and checking which remaining option satisfies ALL stated constraints (not just some) is the reliable tie-breaker for scenario questions.

**Why the others are wrong:**
- Answer length is not a reliable signal on Oracle exams and is a common myth.
- Alphabetical order has no relationship to correctness.
- Each question is self-contained; cross-referencing unrelated questions is a trap that leads to wrong answers.

> ⚠️ Frequently missed on the exam — read the options carefully.

</details>

---

