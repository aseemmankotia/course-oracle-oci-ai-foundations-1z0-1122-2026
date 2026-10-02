## Chapter 6: Generative AI & LLMs Part 1: Generative vs Discriminative, Tokens, Embeddings & Context — Practice Questions

**Q1.** A retail company wants an AI system that can classify customer support tickets into categories like 'billing', 'technical', or 'shipping'. Which type of model is BEST suited for this task?

A) A discriminative model that predicts a category label
B) A generative model that produces new ticket text
C) A diffusion model that generates images of tickets
D) An autoregressive model that completes ticket sentences

<details>
<summary>Answer</summary>

**Correct: A**

Classifying input into a fixed set of labels is a prediction/classification task — the defining job of a discriminative (predictive) model, which learns a decision boundary between classes.

**Why the others are wrong:**
- Generative models are designed to create new content, not assign existing input to a category
- Diffusion models generate images from noise; classification is not their purpose
- Autoregressive text completion generates new tokens; it doesn't map input to a fixed label

> ⚠️ Frequently missed on the exam — read the options carefully.

</details>

---

**Q2.** Which statement correctly distinguishes generative models from discriminative models?

A) Generative models learn P(label | input); discriminative models learn P(input | label)
B) Generative models can only process images; discriminative models can only process text
C) Discriminative models require more training data than generative models in all cases
D) Generative models learn the joint distribution of data and can create new samples; discriminative models learn to separate classes and predict labels

<details>
<summary>Answer</summary>

**Correct: D**

Generative models model how data is produced (often P(input, label) or P(input)) enabling new-content creation; discriminative models learn P(label | input) to classify/predict.

**Why the others are wrong:**
- This reverses the actual probability relationships associated with each model type
- Both model types can operate on text, images, audio, or other data — modality is not the distinguishing factor
- Data requirements depend on the specific architecture and task, not a fixed rule tied to model category

> ⚠️ Frequently missed on the exam — read the options carefully.

</details>

---

**Q3.** An LLM is generating a response one piece at a time, using everything generated so far to decide what comes next. What is each of these individual pieces called?

A) A token
B) A parameter
C) An embedding
D) A checkpoint

<details>
<summary>Answer</summary>

**Correct: A**

LLMs generate text token-by-token; a token is a unit of text (word, subword, or character sequence) produced by the tokenizer that the model predicts one at a time.

**Why the others are wrong:**
- A parameter is a learned weight inside the model, not a unit of generated text
- An embedding is a vector representation of a token's meaning, not the generated unit itself
- A checkpoint is a saved snapshot of model weights during training, unrelated to text generation units

</details>

---

**Q4.** A developer sends a prompt plus a long document to an LLM, and the total exceeds the model's context window. What is the MOST likely result?

A) The model automatically upgrades its context window to fit the input
B) The input is truncated or rejected, and content beyond the limit may be lost
C) The model processes the input at double the normal speed to compensate
D) The model converts the excess text into additional embeddings with no loss

<details>
<summary>Answer</summary>

**Correct: B**

The context window is a fixed maximum number of tokens the model can consider at once (prompt + response). Exceeding it typically causes truncation, an error, or dropped earlier content.

**Why the others are wrong:**
- Context windows are fixed by the model architecture/deployment and don't self-expand at runtime
- Exceeding the limit does not speed up processing — it causes a hard limit issue
- Embeddings represent meaning for retrieval/similarity; they don't losslessly compress overflow tokens into the active context

> ⚠️ Frequently missed on the exam — read the options carefully.

</details>

---

**Q5.** A company wants to build a system that finds semantically similar support articles even when the wording differs (e.g., 'reset password' vs 'can't log in'). Which capability should the system rely on?

A) Token counting
B) Discriminative classification
C) Context window expansion
D) Embeddings representing meaning as vectors

<details>
<summary>Answer</summary>

**Correct: D**

Embeddings map text to numerical vectors such that semantically similar text is close in vector space, enabling similarity search regardless of exact wording.

**Why the others are wrong:**
- Token counting only measures length, not meaning or similarity
- Discriminative classification assigns fixed labels; it doesn't measure semantic closeness between free-text phrases
- Context window size affects how much text a model can process, not how similarity between texts is computed

</details>

---

**Q6.** Which of the following BEST describes how tokenization affects an LLM's input?

A) Tokenization compresses text into images for faster GPU processing
B) Tokenization removes all punctuation and stop words permanently from the input
C) Tokenization translates the input into a fixed target language before processing
D) Tokenization converts raw text into numerical IDs representing words or subwords for the model to process

<details>
<summary>Answer</summary>

**Correct: D**

Tokenization splits text into tokens (words, subwords, or characters) and maps each to a numerical ID, which is the format LLMs actually process.

**Why the others are wrong:**
- Tokenization has nothing to do with converting text into image data
- Tokenization does not selectively strip punctuation or stop words as a rule — it segments all text into tokens
- Tokenization is not a translation step; it works within the same language of the input

</details>

---

**Q7.** During text generation, an LLM outputs a probability distribution over its entire vocabulary before choosing the next word. What is this step fundamentally computing?

A) The probability of each possible next token given the tokens so far
B) The final grammar-checked sentence
C) A discriminative classification of the input's sentiment
D) The embedding vector for the entire document

<details>
<summary>Answer</summary>

**Correct: A**

Autoregressive LLMs predict the next token by computing a probability distribution over the vocabulary conditioned on all preceding tokens, then sampling or selecting the most likely one.

**Why the others are wrong:**
- Grammar checking is not how token prediction works — it's a probabilistic next-token estimation process
- Sentiment classification is a discriminative task unrelated to autoregressive generation
- Embeddings represent meaning for input tokens/context, not the output probability distribution for next-token choice

> ⚠️ Frequently missed on the exam — read the options carefully.

</details>

---

**Q8.** Which best defines 'Generative AI' as tested on the exam?

A) AI that only labels or scores existing data without producing anything new
B) AI limited strictly to generating images from noise using diffusion
C) AI that creates new content such as text, images, or code rather than merely predicting a category
D) AI that only performs numerical forecasting on time-series data

<details>
<summary>Answer</summary>

**Correct: C**

Generative AI refers to models that produce new content (text, images, audio, code, etc.) rather than simply classifying or predicting a label for existing input.

**Why the others are wrong:**
- This describes discriminative/predictive AI, the opposite of generative AI
- Diffusion-based image generation is one example of generative AI, not its full definition
- Time-series forecasting is a predictive task, not the defining scope of generative AI

</details>

---

