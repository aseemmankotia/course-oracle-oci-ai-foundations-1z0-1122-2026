# Answer Key — Practice Test 2

**Q1. Correct: A**

Forecasting uses historical time-series data, seasonality, and external indicators to predict future numeric values such as prices — exactly what's described here.

---

**Q2. Correct: D**

Narrow (weak) AI is built for specific tasks like image recognition or language translation. General (strong) AI, a still-hypothetical concept, would match or exceed human cognitive flexibility across any domain.

---

**Q3. Correct: D**

Because the new system learns patterns from historical data rather than relying on a static, hardcoded threshold, it fits machine learning-based anomaly detection — a core distinction tested on the exam between rule-based automation and AI.

---

**Q4. Correct: C**

When a model perpetuates unfair outcomes because its training data encodes historical human bias, this is algorithmic/data bias — a core responsible-AI risk emphasized on the exam.

---

**Q5. Correct: D**

Counting distinct people requires locating and identifying multiple individual instances within a frame, which is the defining capability of object detection — not just labeling the whole image.

---

**Q6. Correct: B**

A large gap between very high training accuracy and much lower test accuracy is the classic signature of overfitting: the model has fit noise/idiosyncrasies of the training set rather than the general pattern, so it fails to generalize to unseen data.

---

**Q7. Correct: A**

The scenario describes an agent interacting with an environment, taking actions, and receiving reward/penalty signals rather than labeled input-output pairs. This trial-and-error, reward-driven learning process is the defining characteristic of reinforcement learning.

---

**Q8. Correct: D**

Since there are no predefined labels and the goal is to discover natural groupings based on similarity, this is a clustering problem, which falls under unsupervised learning.

---

**Q9. Correct: B**

On highly imbalanced datasets, a naive model that always predicts the majority class can achieve high accuracy while providing zero value for detecting the minority (and often more important) class, which is why accuracy alone can be a misleading conceptual metric in such cases.

---

**Q10. Correct: A**

Transforming raw data (timestamps) into derived, more informative inputs (day of week, hour, time since last transaction) to improve model performance is the definition of feature engineering, a preparation step that occurs before training.

---

**Q11. Correct: D**

Holding out a test set that the model never sees during training allows an unbiased evaluation of generalization performance on unseen data, which is the primary reason for the train/test split in the ML workflow.

---

**Q12. Correct: C**

A large gap between high training accuracy and low test accuracy is the classic signature of overfitting, where the model has learned noise and specific details of the training set rather than generalizable patterns.

---

**Q13. Correct: A**

Unsupervised learning discovers patterns and groupings (clustering) in unlabeled data, which fits the scenario of segmenting customers without predefined category labels.

---

**Q14. Correct: A**

Feature preparation (cleaning, transforming, and selecting relevant variables) happens after raw data is collected and before the model is trained, so the data is in a usable format for learning.

---

**Q15. Correct: D**

Reinforcement learning involves an agent taking actions in an environment and learning through reward and penalty signals over repeated interactions, exactly as described with the robot receiving positive and negative feedback.

---

**Q16. Correct: B**

RNNs and related sequence models are designed to handle ordered, time-dependent data by maintaining a hidden state that captures information from prior steps, which fits time-series forecasting.

---

**Q17. Correct: D**

Depth allows the network to build hierarchical representations, where early layers learn simple features and later layers combine them into increasingly abstract concepts, which is a core reason deep learning outperforms shallow models on complex data.

---

**Q18. Correct: C**

Classical ML algorithms are well suited for small, structured datasets where interpretability and fast training matter, since deep learning typically requires large amounts of data to outperform simpler models.

---

**Q19. Correct: D**

Self-attention is the core mechanism in transformers that allows every token to attend to every other token in the sequence simultaneously, capturing long-range dependencies without sequential processing.

---

**Q20. Correct: B**

The vanishing gradient problem occurs when gradients shrink as they propagate backward through many layers, and using activation functions like ReLU (instead of sigmoid or tanh, which saturate) helps mitigate this by maintaining stronger gradient flow.

---

**Q21. Correct: B**

CNNs use convolutional filters that scan across an image to detect local spatial patterns such as edges, textures, and shapes, making them the architecture specifically designed for image data like X-rays.

---

**Q22. Correct: D**

Transformers use self-attention mechanisms that allow every token to directly attend to every other token in the sequence, regardless of distance, avoiding the vanishing gradient and long-range dependency problems that plague basic RNNs. This is why transformers are the foundation of modern large language models and are well-suited to tasks like long-document translation.

---

**Q23. Correct: C**

Churn prediction assigns an existing label (churn/no-churn) to input data, which is the defining behavior of a discriminative model. Writing a new marketing email from a brief produces novel content, which is the defining behavior of a generative model.

---

**Q24. Correct: A**

Embeddings map tokens into dense numerical vectors positioned in a continuous space such that semantically similar tokens end up close together, which is what enables the model to reason about meaning and similarity.

---

**Q25. Correct: A**

A low temperature makes token sampling favor the most probable next token, producing more deterministic, consistent output — exactly what is needed for repeatable legal summaries.

---

**Q26. Correct: C**

RAG retrieves the most current guideline content from an external knowledge store at query time and grounds the response in those retrieved passages, avoiding retraining and enabling traceable source citations.

---

**Q27. Correct: A**

AI agents extend an LLM with the ability to call external tools (like an API), reason over intermediate results, plan next steps, and take autonomous multi-step actions — exactly matching the described escalation-and-reply workflow.

---

**Q28. Correct: A**

Hallucinated citations occur because the model generates plausible-sounding text without factual grounding. RAG anchors responses in a verified external source, and instructing the model to cite only retrieved content directly addresses the root cause.

---

**Q29. Correct: C**

RAG retrieves relevant, up-to-date documents from an external knowledge store at inference time and injects them into the prompt as grounding context, so the assistant reflects the latest policies without any model retraining, making it ideal for frequently changing content.

---

**Q30. Correct: B**

OCI Data Science Model Deployment takes a registered model artifact from the Model Catalog and exposes it as a managed HTTP endpoint with autoscaling, giving the team full control over their custom model while OCI manages the serving infrastructure.

---

**Q31. Correct: A**

OCI Superclusters connect bare metal GPU instances using RDMA-based cluster networking, delivering the ultra-low-latency, high-throughput interconnect required for distributed training of very large foundation models at massive GPU scale.

---

**Q32. Correct: A**

Select AI in Oracle Database 23ai integrates generative AI directly into the database so analysts can ask natural-language questions that are translated into SQL and executed against the data in place, with no data movement required.

---

**Q33. Correct: B**

OCI Generative AI dedicated AI clusters come in two types: fine-tuning clusters, which are provisioned specifically to customize a base model on isolated, tenant-specific compute, and hosting clusters, which serve inference. Fine-tuning requires the fine-tuning cluster type.

---

**Q34. Correct: C**

OCI AI Services expose ready-to-use, pretrained APIs for specific tasks like vision, speech, and language, whereas OCI Generative AI focuses on large language models for generative tasks (chat, summarization, text generation) and supports optional fine-tuning.

---

**Q35. Correct: B**

OCI AI Services Anomaly Detection is a pretrained, ready-to-use API designed specifically to identify unusual patterns in time-series sensor data, requiring no in-house data science expertise or model building.

---

**Q36. Correct: B**

Oracle Database 23ai includes built-in machine learning (Oracle Machine Learning) that allows training and scoring models directly on data stored in the database, avoiding data movement and separate infrastructure.

---

**Q37. Correct: D**

OCI Document Understanding is purpose-built to extract text, tables, and key-value pairs from scanned documents like invoices and bills of lading using pretrained models, requiring no custom training.

---

**Q38. Correct: B**

OCI Speech converts audio to text and supports speaker diarization, which labels transcript segments by speaker, exactly the capability needed here.

---

**Q39. Correct: D**

OCI Anomaly Detection is built on the Multivariate State Estimation Technique (MSET2), which models correlations between multiple signals to detect subtle anomalies earlier than univariate threshold methods.

---

**Q40. Correct: D**

OCI Forecasting is designed specifically to generate future predictions from historical time-series operational data, such as demand forecasting from consumption history.

---

**Q41. Correct: B**

OCI AI Services, including Language, expose REST APIs and are also accessible via language SDKs (including Python), allowing direct programmatic integration into applications.

---

**Q42. Correct: B**

OCI Language includes a pretrained PII detection capability that identifies and can mask sensitive entities such as names, phone numbers, and SSNs within free text.

---

**Q43. Correct: B**

OCI Document Understanding is purpose-built with pretrained models for extracting key-value pairs, tables, and signatures from documents like invoices, receipts, and forms, and also supports document classification and text extraction.

---

**Q44. Correct: C**

OCI Anomaly Detection uses a multivariate approach (based on the MSET-2 algorithm) that models correlated signals together, making it suited to detecting abnormal behavior across interdependent sensor streams in industrial equipment.

---

**Q45. Correct: C**

OCI Speech supports real-time (streaming) transcription, which processes audio continuously and returns text with minimal latency — required for live captioning use cases.

---

**Q46. Correct: C**

Dedicated AI clusters used to host a fine-tuned custom model require a minimum commitment of 744 unit-hours (equivalent to 31 days) per unit, and billing continues for that commitment whether or not the cluster is actively serving inference traffic.

---

**Q47. Correct: C**

OCI Generative AI Agents implement RAG, retrieving current information from a connected knowledge base (e.g., Oracle 23ai Vector Search or OCI Search with OpenSearch) at query time, so answers stay accurate as source documents change without any retraining.

---

**Q48. Correct: A**

COSINE similarity (measuring the angle between vectors rather than magnitude) is the recommended and most commonly used metric for embeddings from transformer-based models like OCI's Cohere embedding models, since it captures semantic similarity independent of vector length.

---

**Q49. Correct: C**

OCI Generative AI Agents support multiple knowledge base data store types for RAG, including Oracle Database 23ai with AI Vector Search and OCI Search with OpenSearch, in addition to Object Storage for unstructured documents — allowing exactly the mixed structured/unstructured scenario described.

---

**Q50. Correct: A**

T-Few is OCI's parameter-efficient fine-tuning method that updates only a small fraction of model weights (added transformer layers), making it faster and cheaper, and it is explicitly recommended for smaller, narrower training datasets like this scenario's 200 examples.

---

