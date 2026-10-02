## Chapter 5: Deep Learning Foundations Part 2: CNNs, RNNs, Transformers & When to Use DL — Practice Questions

**Q1.** A manufacturing company wants to automatically flag defective parts from photos taken on the assembly line. Which architecture family is BEST suited for this task?

A) Convolutional Neural Network (CNN)
B) Recurrent Neural Network (RNN)
C) Transformer with self-attention only
D) Classical decision tree ensemble

<details>
<summary>Answer</summary>

**Correct: A**

CNNs use convolutional filters to detect local spatial patterns (edges, textures, shapes) and are the standard architecture for image classification and defect detection.

**Why the others are wrong:**
- RNNs are designed for sequential/temporal data, not spatial image data.
- Transformers can process images (via patches) but are not the foundational, exam-tested default for straightforward image classification.
- Decision trees don't scale well to raw pixel data and lack the spatial feature extraction CNNs provide.

</details>

---

**Q2.** A company wants to predict the next value in a stream of sensor readings, where each reading depends on the previous several readings in order. Which architecture family is designed for this kind of data?

A) Recurrent Neural Network (RNN)
B) Convolutional Neural Network (CNN)
C) Random Forest
D) K-Means clustering

<details>
<summary>Answer</summary>

**Correct: A**

RNNs maintain a hidden state that carries information across time steps, making them well suited to sequential/temporal data such as sensor streams.

**Why the others are wrong:**
- CNNs are optimized for spatial data like images, not ordered sequences.
- Random Forest treats each input as independent and has no notion of sequence order.
- K-Means is an unsupervised clustering method, not a sequence predictor.

> ⚠️ Frequently missed on the exam — read the options carefully.

</details>

---

**Q3.** A team is building a system that must understand relationships between words that are far apart in a long document, without processing the text strictly one token at a time. Which architecture is designed to capture these long-range dependencies efficiently?

A) Recurrent Neural Network (RNN)
B) Convolutional Neural Network (CNN)
C) Transformer
D) Support Vector Machine (SVM)

<details>
<summary>Answer</summary>

**Correct: C**

Transformers use self-attention to weigh the relevance of every token to every other token in parallel, capturing long-range dependencies better than sequential RNNs.

**Why the others are wrong:**
- RNNs process tokens sequentially and struggle with very long-range dependencies due to vanishing gradients.
- CNNs capture local patterns via limited receptive fields and are not the standard choice for long-range text dependencies.
- SVMs are classical ML classifiers with no built-in mechanism for sequence or attention modeling.

</details>

---

**Q4.** Modern large language models such as GPT-style models are built on which core architecture?

A) Convolutional Neural Network
B) Transformer
C) Recurrent Neural Network
D) Decision Tree

<details>
<summary>Answer</summary>

**Correct: B**

The Transformer architecture, introduced for its self-attention mechanism, is the foundation of modern large language models.

**Why the others are wrong:**
- CNNs are used for image tasks, not the core architecture of modern LLMs.
- RNNs preceded Transformers and are largely replaced by them for large-scale language modeling.
- Decision trees are classical ML models unrelated to language model architecture.

</details>

---

**Q5.** A team has a small tabular dataset (500 rows, 10 numeric features) and needs a model that is accurate and easy to explain to business stakeholders. Which approach is MOST appropriate?

A) Train a deep Transformer model from scratch
B) Use a classical ML model such as a decision tree or gradient boosting
C) Train a deep CNN on the tabular data
D) Use a large RNN with multiple stacked layers

<details>
<summary>Answer</summary>

**Correct: B**

With small, structured/tabular data and a need for interpretability, classical ML methods typically outperform deep learning, which requires large data volumes and is harder to interpret.

**Why the others are wrong:**
- Transformers require large amounts of data and compute; they are overkill and prone to overfitting on 500 rows.
- CNNs are designed for spatial data like images and don't natively fit unstructured tabular rows.
- RNNs are for sequential data, not independent tabular rows, and also need more data than available.

> ⚠️ Frequently missed on the exam — read the options carefully.

</details>

---

**Q6.** In the self-attention mechanism used by Transformers, each token's representation is computed by comparing which three vectors?

A) Query, Key, Value
B) Filter, Stride, Padding
C) Encoder, Decoder, Embedding
D) Gate, Cell, Hidden state

<details>
<summary>Answer</summary>

**Correct: A**

Self-attention computes a weighted combination of Value vectors, where weights come from the compatibility (dot product) between Query and Key vectors for each token pair.

**Why the others are wrong:**
- Filter, Stride, Padding are CNN convolution hyperparameters, not attention components.
- Encoder/Decoder/Embedding are higher-level Transformer components, not the attention calculation itself.
- Gate, Cell, Hidden state describe RNN/LSTM internals, not Transformer self-attention.

> ⚠️ Frequently missed on the exam — read the options carefully.

</details>

---

**Q7.** Which operation is fundamental to how a CNN detects local spatial patterns such as edges and textures in an image?

A) Recurrent hidden state updates
B) Self-attention weighting
C) K-means centroid assignment
D) Convolution using learned filters

<details>
<summary>Answer</summary>

**Correct: D**

CNNs slide small learned filters (kernels) across the image, computing convolutions that detect local patterns like edges, which are then combined into higher-level features in deeper layers.

**Why the others are wrong:**
- Recurrent hidden state updates are used in RNNs for sequential data, not spatial images.
- Self-attention weighting is the Transformer mechanism, not the core CNN operation.
- K-means centroid assignment is an unsupervised clustering technique unrelated to CNN feature extraction.

</details>

---

**Q8.** Which factor is the STRONGEST justification for choosing deep learning over classical machine learning for a given business problem?

A) The business wants a model that is easy to explain to non-technical stakeholders
B) The dataset is small and highly structured with clear numeric features
C) The data is unstructured (images, audio, or raw text) and large volumes of labeled data are available
D) The team needs the fastest possible training time on limited compute

<details>
<summary>Answer</summary>

**Correct: C**

Deep learning excels when working with unstructured data (images, audio, text) and shines when large volumes of data are available to learn hierarchical features automatically.

**Why the others are wrong:**
- Deep learning models are generally harder to explain than classical ML models, so interpretability favors classical ML.
- Small, structured datasets are better suited to classical ML, which needs less data and is less prone to overfitting.
- Deep learning models typically require more compute and longer training time than classical ML, not less.

</details>

---

