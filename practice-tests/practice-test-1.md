# Practice Test 1: OCI 2025 AI Foundations Associate (1Z0-1122-25) Prep

- **Questions:** 47
- **Time limit:** 90 minutes
- **Passing score:** 70%%

> Answers are in `answer-key-1.md`. Track results in `score-tracker.md`.

---

**Q1.** A retail company has three years of monthly sales data for each product and wants a model that predicts next quarter's demand for inventory planning. Which AI task category BEST fits this requirement?

A) Anomaly detection
B) Recommendation
C) Speech recognition
D) Forecasting

---

**Q2.** A manufacturing plant installs cameras on its assembly line to automatically flag products with surface scratches before they are packaged. Which AI capability is being applied?

A) Computer vision
B) Natural language processing
C) Speech-to-text
D) Time-series forecasting

---

**Q3.** Which statement correctly distinguishes narrow AI from general AI?

A) Narrow AI can only run in the cloud, while general AI can only run on-premises.
B) Narrow AI requires no training data, while general AI requires massive labeled datasets.
C) Narrow AI is designed to perform a specific task well, while general AI would match human-level intelligence across any task.
D) Narrow AI refers to deep learning models, while general AI refers to traditional rule-based systems.

---

**Q4.** A company builds an AI system to screen job applicant resumes and, after deployment, finds it consistently ranks candidates from certain universities lower regardless of qualifications. This outcome is an example of which AI limitation?

A) Insufficient GPU compute for inference
B) A network latency issue in the API gateway
C) Overfitting to the validation dataset only
D) Model bias inherited from training data

---

**Q5.** A telecom company wants customers to be able to ask a chatbot billing questions in plain English and receive accurate written responses. Which AI capability should the solution be built around?

A) Speech synthesis
B) Recommendation engine
C) Image classification
D) Natural language processing

---

**Q6.** A real estate analytics team has a labeled dataset of past home sales, including features like square footage, location, and the actual sale price for each home. They want to build a model that predicts the sale price of a new home based on its features. Which machine learning paradigm BEST fits this task?

A) Supervised learning (regression), since the model learns from labeled data to predict a continuous numeric value
B) Reinforcement learning, since the model needs to learn from feedback over many iterations
C) Unsupervised learning, since the goal is to find patterns in the housing data
D) Supervised learning (classification), since the model assigns homes to price categories

---

**Q7.** A retail company has a large database of customer purchase histories but no predefined categories or labels for customer types. They want to discover natural groupings of similar customers based on purchasing behavior, without specifying in advance what those groups should look like. Which approach BEST addresses this requirement?

A) Unsupervised learning using clustering to group customers based on behavioral similarity
B) Supervised classification using customer purchase history as labeled training data
C) Reinforcement learning to reward the model for correctly assigning customers to segments
D) Supervised regression to predict each customer's total future spending

---

**Q8.** An autonomous robot is placed in a warehouse and must learn to navigate to a charging station. It has no labeled dataset of correct paths; instead, it receives a positive signal when it moves closer to the station and a negative signal when it collides with obstacles. Over many trial runs, it improves its navigation strategy. Which learning paradigm does this describe?

A) Unsupervised learning, since there is no labeled data available
B) Supervised learning, since the robot receives signals indicating correct and incorrect behavior
C) Supervised regression, since the robot must predict a continuous distance value to the station
D) Reinforcement learning, since the robot learns through trial and error using reward and penalty signals

---

**Q9.** A data scientist splits a labeled dataset into a training set and a separate test set before building a model. What is the PRIMARY purpose of holding out this test set?

A) To increase the total amount of data available for training the model
B) To evaluate the model's performance on data it has not seen during training, giving a more realistic estimate of how it will perform on new data
C) To reduce the computational cost of training by using fewer examples
D) To ensure the model achieves the highest possible accuracy on the training data

---

**Q10.** A model achieves 99% accuracy on its training data but only 62% accuracy when evaluated on new, unseen data. Which concept BEST describes this situation?

A) Underfitting, because the model failed to learn any patterns from the training data
B) Overfitting, because the model learned patterns and noise specific to the training data that do not generalize to new data
C) Reinforcement learning failure, because the model did not receive enough reward signals
D) A labeling error, because the training and test sets must have been mislabeled

---

**Q11.** A team builds a fraud detection model on a dataset where only 1% of transactions are fraudulent. The model predicts every transaction as 'not fraud' and achieves 99% accuracy. Which evaluation approach would BEST reveal that this model is not actually useful?

A) Reporting only the overall accuracy score, since 99% accuracy indicates strong performance
B) Increasing the size of the training dataset without changing the evaluation metric
C) Examining metrics such as precision and recall, which account for the model's ability to correctly identify the minority fraud class
D) Switching from a test set to evaluating directly on the training set

---

**Q12.** A retail company has a dataset of customer purchase histories with no predefined labels or categories. They want to discover natural groupings of similar customers for targeted marketing. Which type of machine learning is BEST suited for this task?

A) Unsupervised learning, since the goal is to find patterns and groupings in unlabeled data
B) Reinforcement learning, since the model will learn optimal marketing actions through trial and reward
C) Supervised classification, since customers need to be assigned to predefined categories
D) Supervised regression, since the output is a continuous customer value score

---

**Q13.** An activation function in an artificial neural network is applied to the weighted sum of inputs at each neuron. What is its primary purpose?

A) To reduce the number of layers needed in the network
B) To introduce non-linearity so the network can model complex, non-linear relationships in data
C) To normalize the input dataset before training begins
D) To calculate the final loss value for the entire network

---

**Q14.** A retail company wants to build a model to classify product photos into categories such as shoes, bags, and clothing. Which deep learning architecture is BEST suited for this image classification task?

A) Recurrent Neural Network (RNN)
B) Transformer-based language model
C) Convolutional Neural Network (CNN)
D) Classical linear regression

---

**Q15.** A financial services team needs to predict next month's transaction volume using a sequence of the last 24 months of transaction data, where the order of the data points matters. Which deep learning architecture family is designed specifically to handle this type of sequential, order-dependent data?

A) Recurrent Neural Network (RNN)
B) Convolutional Neural Network (CNN)
C) K-means clustering
D) Decision tree ensemble

---

**Q16.** A company has only 500 labeled rows of structured tabular data (numeric and categorical columns) and needs a model that is fast to train and easy to interpret for regulatory reporting. Which approach is MOST appropriate?

A) Build a deep transformer model with billions of parameters
B) Train a deep convolutional neural network from scratch
C) Use a deep recurrent neural network with multiple stacked layers
D) Use a classical machine learning model such as logistic regression or a decision tree

---

**Q17.** As a neural network's depth (number of hidden layers) increases, what benefit does this generally provide when working with complex data such as images or natural language?

A) It allows the network to learn increasingly abstract, hierarchical feature representations at each layer
B) It guarantees the model will never overfit the training data
C) It eliminates the need for large amounts of training data
D) It removes the need for an activation function in the output layer

---

**Q18.** Modern large language models such as those used in generative AI are primarily built on which deep learning architecture, which relies on a mechanism to weigh the relevance of different words in a sequence relative to one another?

A) Convolutional Neural Network (CNN)
B) K-nearest neighbors
C) Transformer architecture
D) Support vector machine

---

**Q19.** A data science team needs to build a model that translates English sentences into French. The model must process words in sequence while capturing long-range dependencies between words that appear far apart in a sentence. Which deep learning architecture family is BEST suited for this task?

A) Convolutional Neural Networks (CNNs)
B) Transformers
C) Decision tree ensembles
D) K-means clustering networks

---

**Q20.** Which statement best distinguishes a generative AI model from a discriminative (predictive) AI model?

A) A generative model can only process numerical data, while a discriminative model can only process text
B) A generative model requires no training data, while a discriminative model requires labeled training data
C) A generative model always runs on GPUs, while a discriminative model always runs on CPUs
D) A generative model produces new content such as text or images, while a discriminative model predicts a label or category for given input data

---

**Q21.** A company's LLM-powered support assistant needs to answer questions using the company's internal knowledge base, which is updated daily with new product documentation. The company wants answers to reflect the latest documents without retraining the model. Which approach BEST meets this requirement?

A) Retrieval-augmented generation (RAG), retrieving relevant documents at query time to ground the model's response
B) Prompt engineering alone, using longer and more detailed instructions
C) Fine-tuning the model daily on the entire updated knowledge base
D) Increasing the model's temperature setting to improve accuracy

---

**Q22.** A team has a large, high-quality labeled dataset of customer service transcripts in a very specific brand voice and wants an LLM to consistently reproduce that exact tone and terminology across all future outputs. Which technique BEST fits this requirement?

A) Retrieval-augmented generation (RAG)
B) Increasing the context window size
C) Zero-shot prompting
D) Fine-tuning the model on the labeled transcript dataset

---

**Q23.** An LLM has a fixed context window measured in tokens. If a user's conversation history plus the new prompt exceeds this limit, what typically happens?

A) The model automatically fine-tunes itself to expand its context window
B) The oldest tokens are truncated or dropped so the input fits within the allowed limit
C) The request is converted into an embedding vector and processed with no token limit
D) The model switches to a discriminative architecture to compress the input

---

**Q24.** A development team wants to build a system that not only generates text responses but also autonomously decides which external tools to call (such as a calculator or database query) and plans multiple steps to complete a task before returning a final answer. Which concept BEST describes this system?

A) An AI agent
B) A basic text completion prompt
C) An embedding model
D) A discriminative classification model

---

**Q25.** Why do large language models sometimes produce hallucinations — confident but factually incorrect statements?

A) The model deliberately lies when it lacks sufficient computing resources
B) Hallucinations only occur when the temperature setting is set to zero
C) The model is intentionally programmed to insert false information for testing purposes
D) The model generates text by predicting the most statistically likely next tokens, without an inherent mechanism to verify factual accuracy

---

**Q26.** A financial services company wants their chatbot to answer questions about the company's proprietary product catalog, which is updated weekly, without retraining the underlying LLM each time the catalog changes. Which approach BEST meets this requirement?

A) Increase the context window size of the LLM to fit the entire catalog
B) Use retrieval-augmented generation to fetch relevant catalog data at query time
C) Fine-tune the model weekly on the updated catalog data
D) Rely on the LLM's pretrained knowledge and prompt it to be more accurate

---

**Q27.** A customer support team wants to automatically extract sentiment and key phrases from thousands of incoming tickets. They have no data scientists on staff and want a solution that works immediately via a simple API call with no model training required. Which OCI service BEST meets this requirement?

A) OCI Data Science
B) OCI Generative AI dedicated fine-tuning cluster
C) OCI Language
D) Select AI in Oracle Database 23ai

---

**Q28.** A retail company stores sales data in Oracle Database 23ai and wants business analysts, who do not know SQL, to ask questions like 'What were total sales in Q3 by region?' and get an answer directly from the database. Which OCI capability should they use?

A) OCI Vision
B) OCI Anomaly Detection
C) Select AI
D) OCI Data Science Model Deployment

---

**Q29.** An industrial company streams sensor readings from factory equipment and wants to automatically flag unusual readings that could indicate equipment failure, without building or training a custom model. Which OCI AI Service is purpose-built for this?

A) OCI Document Understanding
B) OCI Speech
C) OCI Anomaly Detection
D) OCI Generative AI

---

**Q30.** A data science team wants to build a custom deep learning model using PyTorch, train it on GPU compute, track experiments, and deploy the trained model as a managed REST endpoint using their own labeled dataset. Which part of the OCI AI portfolio should they use?

A) OCI Language
B) OCI Data Science
C) Select AI
D) OCI Anomaly Detection

---

**Q31.** A data scientist is setting up a JupyterLab notebook session in OCI Data Science to train a large convolutional neural network and wants training to complete significantly faster than on a standard CPU shape. Which compute shape configuration should they select for the notebook session?

A) A GPU compute shape such as a VM.GPU or BM.GPU shape
B) A standard Always Free eligible CPU shape
C) An Object Storage Standard tier bucket
D) A block volume with the highest IOPS setting

---

**Q32.** What is the fundamental architectural difference between OCI AI Services and OCI Data Science?

A) AI Services only run on-premises while Data Science only runs in OCI Government Cloud regions
B) AI Services are pretrained models consumed via simple API calls, while Data Science is a platform for building, training, and deploying custom models on your own data
C) AI Services require writing Python code for every request, while Data Science requires no coding at all
D) AI Services are limited to Oracle Database workloads, while Data Science is limited to Generative AI workloads

---

**Q33.** A retail company's data science team wants to write custom Python code in Jupyter notebooks, experiment with different algorithms and hyperparameters, and manage the full lifecycle of their own machine learning models on OCI. Which part of the OCI AI portfolio BEST fits this need?

A) OCI Language service
B) OCI Generative AI service
C) OCI Data Science platform
D) Select AI in Oracle Database 23ai

---

**Q34.** A manufacturing company wants to automatically inspect images captured on its assembly line and draw bounding boxes around defective parts so operators can quickly identify problem areas. Which OCI AI Service BEST meets this requirement?

A) OCI Anomaly Detection
B) OCI Document Understanding
C) OCI Vision
D) OCI Language

---

**Q35.** A tax preparation firm receives thousands of scanned paper tax forms and needs to automatically extract labeled fields (such as 'Taxpayer Name' and 'Total Income') along with table data from the forms into structured data. Which OCI AI Service should they use?

A) OCI Document Understanding
B) OCI Speech
C) OCI Forecasting
D) OCI Vision

---

**Q36.** A retail chain has three years of historical monthly sales data and wants to predict expected sales for each store for the next two quarters to plan inventory. Which OCI AI Service is designed for this task?

A) OCI Anomaly Detection
B) OCI Language
C) OCI Vision
D) OCI Forecasting

---

**Q37.** A customer support center records all phone calls and wants to convert the audio recordings into searchable text transcripts, including automatic punctuation. Which OCI AI Service should be used?

A) OCI Anomaly Detection
B) OCI Document Understanding
C) OCI Speech
D) OCI Language

---

**Q38.** An industrial company streams sensor telemetry (temperature, vibration, pressure) from factory equipment and wants to automatically flag unusual readings that may indicate impending equipment failure, without building a custom machine learning model. Which OCI AI Service fits this need?

A) OCI Anomaly Detection
B) OCI Language
C) OCI Vision
D) OCI Speech

---

**Q39.** A developer building a Python application wants to programmatically submit customer reviews to OCI Language for sentiment analysis as part of an automated pipeline, rather than manually testing each review in the OCI Console. Which approach is appropriate?

A) Manually copy and paste each review into the OCI Console's Language service demo page
B) Export the reviews to OCI Object Storage and wait for automatic processing with no code required
C) Use OCI Data Science notebooks exclusively, since Language service APIs cannot be called from external applications
D) Use the OCI SDK for Python (or direct REST API calls) to invoke the Language service programmatically

---

**Q40.** A telecommunications company records thousands of customer support calls daily and wants to automatically convert the audio into text transcripts for compliance archiving and later analysis. Which OCI AI service BEST meets this requirement?

A) OCI Language
B) OCI Speech
C) OCI Document Understanding
D) OCI Vision

---

**Q41.** A manufacturing company collects continuous sensor telemetry (temperature, vibration, pressure) from factory equipment and wants a service that can automatically flag unusual readings that deviate from normal operating patterns, so maintenance teams can investigate potential equipment failures early. Which OCI AI service should they use?

A) OCI Anomaly Detection
B) OCI Forecasting
C) OCI Language
D) OCI Vision

---

**Q42.** A development team wants to embed OCI AI Service capabilities directly into a custom mobile application's backend code so they can programmatically send requests and receive results without manually using the OCI Console. Which access method should they use?

A) Only the OCI Console web interface
B) REST APIs and SDKs
C) OCI Data Science notebooks exclusively
D) Oracle Database 23ai SQL commands only

---

**Q43.** A retail company wants a chatbot that answers customer questions using the latest product manuals stored in Oracle Database 23ai, and the manuals are updated weekly. The company wants the chatbot to always reflect the newest content without retraining a model every week. Which approach BEST meets these requirements?

A) Fine-tune a foundation model in OCI Generative AI using the Vanilla fine-tuning method on the current manuals
B) Deploy a dedicated hosting AI cluster with a fully fine-tuned model and re-fine-tune it every week
C) Use OCI Generative AI Agents with a RAG pattern that retrieves content from AI Vector Search in Oracle Database 23ai at query time
D) Use only prompt engineering on a pretrained model without connecting to any database

---

**Q44.** A company has fine-tuned a custom model in OCI Generative AI and needs exclusive, dedicated GPU compute to host that model for low-latency inference for a single tenant. Which resource should they provision?

A) An OCI Generative AI Agent
B) A dedicated AI cluster of the hosting type
C) A pretrained on-demand foundation model endpoint
D) An Oracle Database 23ai AI Vector Search index

---

**Q45.** Which OCI Generative AI fine-tuning method updates only a small number of additional parameters while keeping the base model's original weights frozen, making it faster and cheaper than full fine-tuning?

A) Vanilla fine-tuning
B) Retrieval-augmented fine-tuning
C) Full-weight fine-tuning
D) T-Few fine-tuning

---

**Q46.** In Oracle Database 23ai, which native data type is used to store vector embeddings so they can be queried with AI Vector Search similarity operations?

A) BLOB
B) VECTOR
C) JSON
D) CLOB

---

**Q47.** A healthcare provider needs to build an internal assistant that answers clinician questions by combining a foundation model's language ability with real-time retrieval from clinical notes stored as vector embeddings in Oracle Database 23ai. Which OCI service is purpose-built to orchestrate this retrieval-augmented generation workflow end to end?

A) OCI Data Science notebook sessions
B) OCI Vision AI service
C) OCI Generative AI Agents
D) OCI Generative AI on-demand embedding endpoint alone, without any agent orchestration

---

