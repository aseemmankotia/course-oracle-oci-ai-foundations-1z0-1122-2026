# Practice Test 2: OCI 2025 AI Foundations Associate (1Z0-1122-25) Prep

- **Questions:** 50
- **Time limit:** 90 minutes
- **Passing score:** 70%%

> Answers are in `answer-key-2.md`. Track results in `score-tracker.md`.

---

**Q1.** A logistics company wants to predict future fuel costs for the next quarter based on historical price trends, seasonal patterns, and market indicators. Which AI task category BEST describes this requirement?

A) Forecasting
B) Anomaly detection
C) Classification
D) Recommendation

---

**Q2.** Which statement correctly distinguishes narrow AI from general AI?

A) General AI is currently the dominant form of AI deployed in enterprises today, while narrow AI remains largely theoretical.
B) Narrow AI and general AI are interchangeable terms describing the same underlying technology.
C) General AI refers only to AI models that use generative techniques, while narrow AI refers strictly to traditional rule-based systems.
D) Narrow AI is designed and trained to perform a specific task or a limited set of tasks, whereas general AI would possess broad, human-like cognitive abilities across any intellectual task.

---

**Q3.** A finance department currently uses a traditional system that flags any invoice over $10,000 for manual review, based on a hardcoded if-then rule. They want to replace it with a system that learns from historical approval patterns to flag unusual invoices even when they fall below that fixed threshold. Which category does the NEW system fall into?

A) A rule-based system, since it still evaluates invoices against some criteria
B) A speech recognition system used to transcribe invoice data
C) A recommendation engine suggesting which invoices to approve
D) Machine learning-based anomaly detection that identifies unusual patterns without relying solely on fixed thresholds

---

**Q4.** A bank deploys a machine learning model to approve or deny loan applications. The model was trained on decades of historical lending data that reflected past discriminatory lending practices, and it now systematically denies loans to certain demographic groups at a higher rate. This is an example of which limitation/risk category?

A) Overfitting to noise in the training data
B) Data drift caused by changing market conditions
C) Algorithmic bias resulting from historical data reflecting past discriminatory practices
D) High inference latency due to model complexity

---

**Q5.** A retailer wants to automatically count how many individual customers are present in a store at any given time by analyzing camera feeds, distinguishing each separate person rather than just labeling the overall scene. Which AI task BEST fits this requirement?

A) Text generation
B) Speech recognition
C) Image classification, which assigns a single label to an entire image
D) Object detection, which identifies and localizes individual instances of objects (in this case, people) within an image or video frame

---

**Q6.** A data science team trains a decision tree that achieves 99% accuracy on the training dataset but only 61% accuracy on a held-out test dataset. Which condition BEST explains this behavior?

A) The model is underfitting because it has not learned the training data well enough
B) The model is overfitting because it has memorized noise and patterns specific to the training data that do not generalize
C) The model is using reinforcement learning and needs more reward signals
D) The model has too few features to learn the underlying pattern

---

**Q7.** An engineering team wants an agent to learn how to balance a robot on two wheels. The agent receives a positive signal when the robot stays upright longer and a negative signal when it falls, with no labeled 'correct action' provided for each state. Which machine learning paradigm does this scenario describe?

A) Reinforcement learning, because the agent learns a policy through trial-and-error using reward and penalty signals
B) Supervised learning, because the agent is being trained on examples
C) Unsupervised learning, because there are no labels in the dataset
D) Regression, because the output is a continuous balance angle

---

**Q8.** A retailer has a dataset of 50,000 customer transactions with no predefined categories or labels. The team wants to discover natural groupings of customers with similar purchasing behavior so they can design different marketing campaigns for each group. Which approach is MOST appropriate?

A) Supervised classification using labeled customer segments from a previous campaign
B) Reinforcement learning to reward the model for correct marketing predictions
C) Linear regression to predict each customer's exact future spend
D) Unsupervised clustering to group customers based on similarity in their purchasing patterns

---

**Q9.** A dataset for detecting a rare disease contains 990 healthy patients and only 10 patients with the disease. A model that simply predicts 'healthy' for every patient achieves 99% accuracy. Why is accuracy alone a poor conceptual choice for evaluating this model?

A) Accuracy can only be calculated for regression problems, not classification problems
B) Accuracy is misleading on imbalanced datasets because a model can score very high while completely failing to identify the minority class of interest
C) Accuracy requires a train/test split to be calculated, which was not performed here
D) Accuracy increases only when the model overfits the training data

---

**Q10.** During an ML workflow, a data scientist takes raw transaction timestamps and converts them into new inputs such as 'day of week', 'hour of day', and 'time since last transaction' before training a fraud detection model. Which step of the machine learning workflow does this represent?

A) Feature engineering, since raw data is being transformed into more informative inputs for the model
B) Model evaluation, since new metrics are being introduced
C) Data collection, since new data is being gathered from an external source
D) Inference, since the model is generating predictions from the new fields

---

**Q11.** A team splits their labeled dataset into 80% for training and 20% for testing before building a classification model. What is the PRIMARY purpose of reserving the 20% test set rather than using all data for training?

A) To increase the total amount of data available for training the model
B) To speed up the training process by reducing the dataset size
C) To eliminate the need for feature engineering on the remaining data
D) To provide an unbiased estimate of how the model will perform on new, unseen data after training is complete

---

**Q12.** A data scientist trains a model that achieves 99% accuracy on training data but only 62% accuracy on new, unseen data. Which concept BEST explains this behavior?

A) The model is underfitting because it has too few parameters to capture patterns
B) The model is using reinforcement learning, which always performs poorly on unseen data
C) The model is overfitting because it memorized the training data instead of learning generalizable patterns
D) The model's train/test split was performed after training, which is the correct approach

---

**Q13.** A retailer wants to group customers into segments based on purchasing behavior, but has no predefined labels for the segments. Which type of machine learning is most appropriate?

A) Unsupervised learning
B) Supervised classification
C) Reinforcement learning
D) Supervised regression

---

**Q14.** In the typical machine learning workflow, feature preparation occurs at which stage?

A) After data collection and before model training
B) After model evaluation, to adjust the accuracy metric
C) During inference, to generate predictions on new data
D) After deployment, to monitor model drift

---

**Q15.** An autonomous robot learns to navigate a warehouse by receiving positive signals when it avoids obstacles and negative signals when it collides with them, adjusting its behavior over many attempts. Which learning paradigm does this describe?

A) Unsupervised learning
B) Supervised regression
C) Supervised classification
D) Reinforcement learning

---

**Q16.** A data science team is building a model to forecast hourly electricity demand using the past 30 days of readings, where each hour's demand depends heavily on the pattern of previous hours. Which deep learning architecture family is most appropriate for this sequential dependency?

A) Convolutional neural networks, because they excel at spatial feature extraction
B) Recurrent neural networks or other sequence models, because they process data with temporal order and retain information across time steps
C) A single-layer perceptron, because demand forecasting is a linear problem
D) Transformers, because they are exclusively designed for natural language text

---

**Q17.** Why does increasing the depth (number of layers) in a neural network generally improve its ability to model complex data, compared to a shallow network with the same total number of neurons?

A) Deeper networks always train faster because gradients propagate more efficiently through more layers
B) Depth has no real effect on model capacity; only the total neuron count matters
C) Deeper networks eliminate the need for activation functions between layers
D) Each additional layer can learn increasingly abstract representations by combining features from previous layers, enabling hierarchical feature learning

---

**Q18.** An analyst has a small structured dataset of 500 rows with 10 numeric features and needs to predict a binary outcome. Model interpretability and fast training time are also required. Which approach is most appropriate?

A) A deep neural network with multiple hidden layers, since deep learning always outperforms classical ML
B) A transformer-based model, since transformers are the current state of the art for all prediction tasks
C) A classical machine learning algorithm such as logistic regression or a decision tree, since the dataset is small, structured, and interpretability is required
D) A convolutional neural network, since CNNs generalize well to any tabular dataset

---

**Q19.** In the transformer architecture that underlies modern large language models, what is the primary mechanism that allows the model to weigh the relevance of different words in a sequence relative to one another, regardless of their distance apart?

A) Recurrent connections that pass hidden states sequentially from one word to the next
B) Convolutional filters that slide across the input sequence
C) Max pooling layers that reduce sequence length before processing
D) Self-attention, which computes relationships between all tokens in a sequence in parallel

---

**Q20.** A team is training a deep neural network and notices that during backpropagation, the gradients in the earliest layers become extremely small, causing those layers to stop learning effectively. What is this phenomenon commonly called, and what architectural element is often adjusted to help address it?

A) Overfitting; the fix is to increase the number of training epochs
B) The vanishing gradient problem; the fix often involves choosing activation functions such as ReLU instead of sigmoid or tanh
C) Exploding gradients; the fix is to reduce the learning rate to zero
D) Underfitting; the fix is to remove hidden layers entirely

---

**Q21.** A company wants to build a system that classifies medical images (X-rays) into categories such as 'normal' or 'pneumonia detected.' Which deep learning architecture family is specifically designed to exploit the spatial structure of image data, such as local pixel patterns and shapes?

A) Recurrent neural networks, because they process data in temporal sequence
B) Convolutional neural networks, because they use filters that detect local spatial patterns like edges and textures
C) Generative adversarial networks, because they are required for any image-related task
D) Transformers only, because they have fully replaced CNNs for all image tasks as of 2025

---

**Q22.** A data science team is building a model to translate lengthy legal documents from English to French, where correctly translating a word often depends on context from sentences much earlier or later in the document. Early experiments with a basic recurrent neural network produced poor translations for long documents due to loss of context over long sequences. Which deep learning architecture family BEST addresses this requirement?

A) A convolutional neural network (CNN), since it can scan the entire document in parallel using filters
B) A basic recurrent neural network (RNN) with a larger hidden state size to store more context
C) A classical machine learning algorithm such as a decision tree trained on hand-crafted linguistic features
D) A transformer architecture using self-attention to directly relate tokens regardless of their distance in the sequence

---

**Q23.** A retail company has two AI initiatives: (1) a model that predicts whether a customer will churn based on historical account data, and (2) a model that writes personalized marketing emails from a short brief. Which statement correctly classifies these two models?

A) Both are generative models because they both produce output based on input data
B) Initiative 1 uses a generative model to synthesize churn probabilities; Initiative 2 uses a discriminative model to classify email tone
C) Initiative 1 uses a discriminative model that predicts a label from existing data; Initiative 2 uses a generative model that creates new content
D) Both are discriminative models because they both rely on labeled training data

---

**Q24.** In the context of large language models, what does a token embedding represent?

A) A numerical vector that captures the semantic meaning and relationships of a token in a continuous vector space
B) A compressed version of the original text used only to reduce storage costs
C) A unique identifier number assigned to a token so it can be looked up in a dictionary
D) A hash value used to verify that generated text has not been tampered with

---

**Q25.** You are configuring an OCI Generative AI chat model to draft highly consistent, deterministic legal document summaries where creative variation is undesirable. Which decoding parameter adjustment BEST achieves this goal?

A) Set temperature close to 0 (low value) to make the model favor the highest-probability tokens
B) Increase the temperature toward 1.0 and increase top-p toward 1.0 to allow broader token sampling
C) Increase the max output token length to force the model to generate longer, more detailed summaries
D) Disable the context window so the model relies only on the current prompt

---

**Q26.** A healthcare provider wants its chatbot to answer questions using the latest internal clinical guidelines, which are updated weekly. The provider does not want to retrain the model each time content changes and needs verifiable source citations. Which approach BEST meets these requirements?

A) Fine-tune the LLM weekly on the updated clinical guideline documents
B) Increase the temperature parameter so the model generates more varied and creative answers
C) Use retrieval-augmented generation (RAG) to retrieve the current guideline content from a vector store and ground the model's responses at query time
D) Expand the context window size so the entire guideline library can be pasted into every prompt

---

**Q27.** A company wants to build an AI assistant that can autonomously check a customer's order status by calling an internal REST API, decide whether to escalate the issue based on the API response, and then compose a reply email — all without a human specifying each step. Which capability BEST describes what is needed?

A) An AI agent that combines an LLM with tool-calling and multi-step reasoning/planning to decide and execute actions
B) A single-turn prompt to a foundation model with a longer context window
C) A fine-tuned model trained only on customer email examples
D) A retrieval-augmented generation pipeline that only fetches static FAQ documents

---

**Q28.** An LLM-powered chatbot deployed for a law firm frequently fabricates case citations that sound plausible but do not exist. Which action would MOST effectively reduce this hallucination behavior while preserving the chatbot's ability to answer legal questions?

A) Ground the model's responses using retrieval-augmented generation against a verified legal case database, and instruct it to only cite retrieved sources
B) Increase the temperature setting so the model produces more diverse citation formats
C) Remove the system prompt entirely so the model relies solely on its pretraining knowledge
D) Reduce the model's maximum output token limit so it generates shorter answers

---

**Q29.** A financial services firm's internal knowledge base of compliance policies changes weekly. The firm wants its LLM-based assistant to always answer using the most current policy text, without incurring the cost and delay of retraining the model every time a policy changes. Which approach BEST satisfies this requirement?

A) Fine-tune the model on the full policy corpus every week before deployment
B) Increase the model's context window size so the entire policy corpus can be pasted into every prompt
C) Implement retrieval-augmented generation so the model retrieves and grounds responses in the current policy documents at query time
D) Rely on the model's pretraining knowledge and use few-shot prompting with example Q&A pairs

---

**Q30.** A data science team already has a model trained with scikit-learn and wants to deploy it as an HTTP endpoint with autoscaling for real-time inference, while retaining full control of the model artifact inside their own OCI tenancy. Which OCI Data Science capability directly fits this need?

A) OCI AI Services Vision
B) OCI Data Science Model Deployment
C) OCI Generative AI dedicated fine-tuning cluster
D) Select AI in Oracle Database 23ai

---

**Q31.** An organization needs to train a 70-billion parameter foundation model from scratch and requires ultra-low-latency interconnect between thousands of GPUs distributed across multiple bare metal hosts. Which OCI infrastructure capability is specifically designed to meet this requirement?

A) OCI Supercluster with RDMA-based cluster networking connecting bare metal GPU instances
B) OCI Compute VM.Standard shapes with block storage
C) OCI Autonomous Database with in-memory column store
D) OCI AI Services Document Understanding batch processing

---

**Q32.** A company wants business analysts to query their Oracle Database 23ai tables using plain natural-language questions, with the database automatically translating the question into SQL and returning results, without moving the data out of the database. Which OCI AI capability should they use?

A) Select AI in Oracle Database 23ai
B) OCI Generative AI dedicated fine-tuning cluster
C) OCI Data Science Model Catalog
D) OCI AI Services Language entity extraction

---

**Q33.** In the OCI Generative AI service, an enterprise wants to fine-tune a pretrained foundation model using their own labeled dataset while ensuring the base model weights used during training are isolated from other tenants. Which resource must they provision?

A) A hosting dedicated AI cluster
B) A fine-tuning dedicated AI cluster
C) An AI Quick Actions notebook session
D) A shared on-demand inference endpoint

---

**Q34.** Which statement accurately distinguishes OCI AI Services from the OCI Generative AI service?

A) OCI AI Services can only be used from inside OCI Data Science notebook sessions, while OCI Generative AI runs completely independently
B) OCI Generative AI is limited to image classification tasks, while OCI AI Services handle only text-based tasks
C) OCI AI Services are pretrained, task-specific APIs (such as vision, speech, and language), while OCI Generative AI provides access to large language models for text generation, summarization, and chat that can also be customized
D) OCI AI Services always require a dedicated GPU cluster, while OCI Generative AI runs solely on CPU-only shapes

---

**Q35.** A logistics company needs to detect unusual patterns in real-time sensor readings from delivery trucks but has no in-house data science team and wants the fastest path to production using a ready-made capability. Which part of the OCI AI portfolio should they use?

A) OCI Data Science, building a custom anomaly detection model from scratch
B) OCI AI Services Anomaly Detection
C) OCI Generative AI, fine-tuning a large language model
D) Select AI in Oracle Database 23ai

---

**Q36.** A retail company wants to build a fraud detection model using their transaction data that already resides in Oracle Database 23ai. They want to train and run inference on this data without moving it to a separate data science environment or standing up new infrastructure. Which OCI AI portfolio capability BEST meets this requirement?

A) OCI Data Science with a managed notebook session and model deployment
B) In-database machine learning capabilities of Oracle Database 23ai (Oracle Machine Learning)
C) OCI Generative AI service with a fine-tuned foundation model
D) OCI Anomaly Detection AI service

---

**Q37.** A logistics company receives thousands of scanned bills of lading and needs to automatically extract key-value pairs such as shipper name, consignee, and shipment date, plus table line items, without first labeling training data. Which OCI AI service BEST meets this requirement?

A) OCI Vision using a custom object detection model
B) OCI Language named entity recognition
C) OCI Data Science with a custom Jupyter notebook pipeline
D) OCI Document Understanding using pretrained key-value extraction

---

**Q38.** A call center wants to transcribe recorded customer service calls and needs the transcript to indicate which speaker (agent or customer) said each sentence. Which OCI AI Service capability enables this?

A) OCI Language sentiment analysis
B) OCI Speech with speaker diarization enabled
C) OCI Anomaly Detection multivariate scoring
D) OCI Vision text detection

---

**Q39.** Which underlying algorithm does OCI Anomaly Detection use to identify anomalies across multiple correlated sensor signals simultaneously in operational data?

A) K-means clustering
B) Convolutional neural network
C) Linear regression
D) Multivariate State Estimation Technique (MSET2)

---

**Q40.** A utility company wants to predict next month's electricity demand using three years of historical hourly consumption data. Which OCI AI service is purpose-built for this task?

A) OCI Vision
B) OCI Anomaly Detection
C) OCI Language
D) OCI Forecasting

---

**Q41.** A developer wants to integrate OCI Language sentiment analysis directly into a Python application without manually using the OCI Console. Which approach is appropriate?

A) Manually copy predictions from the Console UI into the application
B) Call the OCI Language REST API or use the OCI SDK for Python
C) Export a downloadable on-premises binary since OCI AI services cannot be called programmatically
D) Use the OCI Anomaly Detection API as a substitute since both are AI services

---

**Q42.** A healthcare company needs to automatically redact patient names, phone numbers, and social security numbers from free-text clinical notes before sharing the data with a research partner. Which OCI AI service capability directly supports this requirement?

A) OCI Anomaly Detection
B) OCI Language PII detection
C) OCI Vision object detection
D) OCI Speech transcription

---

**Q43.** A logistics firm receives thousands of scanned invoices and shipping manifests. They need to automatically extract key-value pairs (e.g., invoice number, total amount), detect table structures, and locate signature fields, all using a pretrained model without building custom ML pipelines. Which OCI AI Service BEST meets these requirements?

A) OCI Vision
B) OCI Document Understanding
C) OCI Language
D) OCI Data Science

---

**Q44.** An oil refinery collects thousands of correlated readings every second from temperature, pressure, and vibration sensors across interdependent equipment. Operators want a service that models the normal relationships between all signals simultaneously and flags abnormal equipment behavior before failure. Which OCI AI Service should they choose?

A) OCI Forecasting
B) OCI Vision
C) OCI Anomaly Detection
D) OCI Language

---

**Q45.** A media company wants to display live captions on screen as a speaker talks during a broadcast, with minimal delay between spoken words and displayed text. Which OCI Speech processing approach should they configure?

A) Asynchronous (batch) transcription of the full recording after the broadcast ends
B) OCI Language sentiment analysis applied to a pre-transcribed script
C) Real-time (streaming) transcription that returns partial results as audio arrives
D) OCI Document Understanding text extraction on a PDF of the script

---

**Q46.** A company is building a custom fine-tuned OCI Generative AI model on the Cohere Command family and wants to host it in production. The finance team asks how long they must commit to paying for the dedicated hosting AI cluster once it is provisioned. What is the minimum commitment for a dedicated AI cluster used for HOSTING a custom model?

A) 1 unit-hour, billed only while inference requests are actively processed
B) 168 unit-hours (7 days), renewable weekly with no long-term lock-in
C) 744 unit-hours (31 days) per cluster unit, billed regardless of usage
D) There is no minimum commitment; hosting clusters bill per-token like on-demand models

---

**Q47.** An enterprise's internal policy documents are updated multiple times per day, and employees need a chat assistant that always reflects the latest wording without daily retraining costs. Which OCI generative-AI approach BEST fits this requirement?

A) Fine-tune a custom model nightly using OCI Data Science and redeploy it to a dedicated AI cluster each morning
B) Increase the context window of the base model prompt to paste the entire policy manual into every request
C) Use OCI Generative AI Agents with a Retrieval-Augmented Generation (RAG) knowledge base connected to the live document store
D) Use the Vanilla fine-tuning method on a large pretrained model to embed the policy content into model weights permanently

---

**Q48.** A developer generates embeddings for product descriptions using an OCI Generative AI embedding model (e.g., cohere.embed-english-v3.0) and stores them as a VECTOR column in Oracle Database 23ai. When writing a similarity search query with the VECTOR_DISTANCE function, which distance metric does Oracle recommend as the standard choice for comparing embeddings produced by these OCI embedding models?

A) COSINE
B) MANHATTAN
C) HAMMING
D) JACCARD

---

**Q49.** A team wants to deploy an OCI Generative AI Agent that answers customer questions by retrieving information from both structured product data stored as vectors in Oracle Database 23ai and unstructured support articles indexed in a separate search cluster. Which single option correctly describes supported data store integrations for an OCI Generative AI Agent's knowledge base?

A) Only Oracle Object Storage buckets containing PDF files are supported as knowledge bases
B) OCI Generative AI Agents can only connect to on-premises Oracle databases via FastConnect, not Oracle Database 23ai in OCI
C) Oracle 23ai AI Vector Search and OCI Search with OpenSearch can both serve as connected knowledge base data stores for the agent
D) Knowledge bases must first be exported to a fine-tuning dataset before the agent can use them

---

**Q50.** A data scientist has only 200 labeled examples to customize an OCI Generative AI Cohere Command model for a narrow classification task and wants the lowest cost and fastest turnaround. Which fine-tuning approach should they select, and why?

A) T-Few fine-tuning, because it updates only a small subset of transformer layer weights, making it efficient and well-suited to smaller training datasets
B) Vanilla fine-tuning, because updating all model weights guarantees better accuracy regardless of dataset size
C) Full pretraining from scratch, because small datasets require building a new base model to avoid overfitting
D) Prompt engineering only, since OCI Generative AI does not support parameter-efficient fine-tuning methods

---

