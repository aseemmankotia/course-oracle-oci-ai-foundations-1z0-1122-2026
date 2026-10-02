# Answer Key — Practice Test 1

**Q1. Correct: D**

Forecasting uses historical time-series data to predict future numeric values such as demand, revenue, or inventory needs — exactly the described scenario.

---

**Q2. Correct: A**

Computer vision enables machines to interpret and analyze visual input from images or video, which is required to detect physical defects like scratches on a product.

---

**Q3. Correct: C**

Narrow AI (or weak AI) is built and trained for one specific task, such as image classification or translation. General AI (or strong AI) is a theoretical concept describing a system with human-like reasoning across any domain, and it does not yet exist in production systems.

---

**Q4. Correct: D**

When an AI system produces systematically unfair outcomes for certain groups, it typically reflects bias present in the historical training data — a key responsible-AI risk covered in the exam.

---

**Q5. Correct: D**

Natural language processing (NLP) enables systems to understand written human language and generate coherent, relevant text responses, which is exactly what a text-based billing chatbot requires.

---

**Q6. Correct: A**

The dataset contains labeled examples (features paired with a known continuous output, sale price), and the target variable is numeric — this is the classic definition of supervised regression.

---

**Q7. Correct: A**

Clustering, an unsupervised learning technique, discovers natural groupings in unlabeled data based on similarity, which matches the described need with no predefined labels.

---

**Q8. Correct: D**

Reinforcement learning is defined by an agent that learns an optimal policy through interacting with an environment and receiving reward/penalty signals over repeated trials, exactly as described here.

---

**Q9. Correct: B**

The train/test split exists specifically to hold back unseen data so the model's generalization performance can be assessed independently of the data used to fit it, revealing issues like overfitting.

---

**Q10. Correct: B**

A large gap between very high training accuracy and much lower test accuracy is the classic signature of overfitting — the model memorized training-specific patterns and noise rather than learning generalizable relationships.

---

**Q11. Correct: C**

On imbalanced datasets, accuracy alone can be misleading because a model can score high by always predicting the majority class; metrics like precision and recall specifically measure how well the minority (fraud) class is detected.

---

**Q12. Correct: A**

Unsupervised learning is used to find hidden patterns or groupings in data without predefined labels, and clustering is the classic technique for segmenting customers based on similarity.

---

**Q13. Correct: B**

Without activation functions, a neural network would just be a linear transformation regardless of depth. Activation functions (like ReLU, sigmoid) introduce non-linearity, enabling the network to approximate complex, non-linear functions.

---

**Q14. Correct: C**

CNNs use convolutional layers with filters that detect spatial patterns like edges, shapes, and textures, making them the standard architecture for image classification tasks.

---

**Q15. Correct: A**

RNNs (and variants like LSTMs) maintain an internal state that carries information across time steps, making them well-suited for sequential data where order and temporal dependencies matter.

---

**Q16. Correct: D**

With small, structured tabular datasets and a need for interpretability, classical ML models like logistic regression or decision trees train efficiently, require less data, and are more interpretable than deep learning approaches.

---

**Q17. Correct: A**

Deeper networks can learn hierarchical representations, where early layers capture simple patterns (edges, basic features) and deeper layers combine them into increasingly abstract, complex representations, which is key to handling complex data types like images and text.

---

**Q18. Correct: C**

Transformers use a self-attention mechanism that allows the model to weigh relationships between all words in a sequence simultaneously, regardless of their distance apart, forming the foundation of modern LLMs.

---

**Q19. Correct: B**

Transformers use self-attention mechanisms to weigh relationships between all words in a sequence regardless of their distance apart, making them the modern standard for sequence-to-sequence tasks like machine translation and the foundation of modern language models.

---

**Q20. Correct: D**

Generative models learn the underlying distribution of data so they can create new, original outputs (text, images, code), whereas discriminative models learn a decision boundary to classify or predict labels for given inputs.

---

**Q21. Correct: A**

RAG retrieves the most current, relevant external documents at inference time and injects them into the prompt context, letting the model generate grounded answers without any retraining, which is ideal for frequently changing knowledge bases.

---

**Q22. Correct: D**

Fine-tuning adjusts the model's internal weights using a labeled dataset so the model consistently and durably adopts a specific style, tone, or domain vocabulary across all future generations, which is exactly what is needed here.

---

**Q23. Correct: B**

The context window defines the maximum number of tokens (input plus output) an LLM can process at once; when this limit is exceeded, the oldest or excess tokens are typically truncated or dropped so the remaining content fits within the model's fixed limit.

---

**Q24. Correct: A**

An AI agent extends an LLM's capabilities by giving it the ability to reason, plan multi-step actions, and autonomously invoke external tools or APIs to accomplish a goal, rather than simply producing a single text response.

---

**Q25. Correct: D**

LLMs generate text token by token based on learned statistical patterns of language, not on a built-in fact-checking or knowledge-verification process, so they can produce plausible-sounding but incorrect or fabricated content, known as hallucination.

---

**Q26. Correct: B**

RAG retrieves current, relevant information from an external knowledge source at inference time, allowing the model to answer with up-to-date information without any retraining, which fits weekly-changing data perfectly.

---

**Q27. Correct: C**

OCI Language is a pretrained AI Service that performs sentiment analysis and key phrase extraction out of the box via a REST API, requiring no model training or data science expertise.

---

**Q28. Correct: C**

Select AI in Oracle Database 23ai lets users pose natural language questions that are translated into SQL and run against the database, returning results without the user writing SQL.

---

**Q29. Correct: C**

OCI Anomaly Detection is a pretrained AI Service specifically designed to identify anomalies in time series sensor data, such as signals from industrial equipment, without requiring custom model development.

---

**Q30. Correct: B**

OCI Data Science is the platform designed for building, training, and deploying custom machine learning and deep learning models using open-source frameworks like PyTorch, with support for GPU compute shapes, experiment tracking via notebook sessions, and managed model deployment endpoints.

---

**Q31. Correct: A**

OCI Data Science notebook sessions can be configured with GPU compute shapes (such as VM.GPU or BM.GPU series), which dramatically accelerate deep learning training compared to CPU-only shapes because GPUs are optimized for the parallel matrix operations used in neural networks.

---

**Q32. Correct: B**

OCI AI Services provide prebuilt, pretrained models (Language, Vision, Speech, Document Understanding, Anomaly Detection) accessible through straightforward API calls with no training required, whereas OCI Data Science is a full platform where users bring their own data to build, train, tune, and deploy custom machine learning models using frameworks like TensorFlow or PyTorch.

---

**Q33. Correct: C**

OCI Data Science is a managed platform providing JupyterLab notebook sessions, support for open-source frameworks, and tools (models, projects, jobs, model catalog) for building, training, and managing the full lifecycle of custom ML models.

---

**Q34. Correct: C**

OCI Vision provides object detection, which identifies and localizes objects within images using bounding boxes, exactly matching the requirement to visually flag defective parts.

---

**Q35. Correct: A**

OCI Document Understanding is purpose-built to extract text, tables, and key-value pairs from scanned or digital documents such as forms, invoices, and receipts.

---

**Q36. Correct: D**

OCI Forecasting is a pretrained AI service that generates time-series predictions, such as future sales, from historical operational data.

---

**Q37. Correct: C**

OCI Speech is a speech-to-text service that transcribes audio files into text, including features like punctuation and word-level timestamps, making it suitable for transcribing call recordings.

---

**Q38. Correct: A**

OCI Anomaly Detection is a pretrained service designed to detect anomalies in multivariate time-series operational and sensor data, ideal for identifying abnormal equipment readings.

---

**Q39. Correct: D**

OCI AI Services, including Language, can be consumed programmatically through language-specific SDKs (such as the OCI SDK for Python) or by directly calling the REST API, enabling automated integration into applications and pipelines.

---

**Q40. Correct: B**

OCI Speech converts audio (speech) into accurate text transcripts and supports batch processing of audio files, which fits the call transcription and archiving use case directly.

---

**Q41. Correct: A**

OCI Anomaly Detection is purpose-built to identify unusual data points or patterns in time-series operational data such as sensor telemetry, making it ideal for detecting abnormal equipment behavior for predictive maintenance.

---

**Q42. Correct: B**

OCI AI Services expose REST APIs, and Oracle provides SDKs in multiple languages, allowing developers to call these services programmatically from custom applications, which is the standard way to integrate AI capabilities into production software.

---

**Q43. Correct: C**

RAG with OCI Generative AI Agents retrieves current content directly from AI Vector Search in Oracle Database 23ai at query time, so answers automatically reflect the latest manuals without any retraining.

---

**Q44. Correct: B**

OCI Generative AI dedicated AI clusters come in two types, fine-tuning and hosting; a hosting dedicated AI cluster provides dedicated, isolated GPU compute to serve a custom fine-tuned model for a single customer.

---

**Q45. Correct: D**

T-Few is the parameter-efficient fine-tuning method offered by OCI Generative AI; it inserts and trains a small set of additional parameters while the base model weights remain frozen, reducing training time and cost.

---

**Q46. Correct: B**

Oracle Database 23ai introduces the native VECTOR data type specifically to store embeddings, enabling AI Vector Search to perform similarity searches (e.g., cosine, dot product, Euclidean) directly in SQL.

---

**Q47. Correct: C**

OCI Generative AI Agents is purpose-built to orchestrate RAG workflows, connecting a foundation model to a knowledge base such as AI Vector Search in Oracle Database 23ai to retrieve relevant context and generate grounded answers.

---

