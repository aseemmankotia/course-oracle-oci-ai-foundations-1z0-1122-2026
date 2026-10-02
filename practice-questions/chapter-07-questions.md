## Chapter 7: Generative AI & LLMs Part 2: Prompt Engineering, RAG, Fine-Tuning & Agents — Practice Questions

**Q1.** A company's internal chatbot must answer employee questions about HR policies that are updated every week. The company wants the chatbot to always reflect the latest policy text without retraining a model each time a policy changes. Which approach BEST meets this requirement?

A) Fine-tune the base model weekly on the updated policy documents
B) Increase the model's temperature setting so it generates more varied answers
C) Use zero-shot prompting with no additional context
D) Use Retrieval-Augmented Generation (RAG) to retrieve current policy documents at query time and ground the response

<details>
<summary>Answer</summary>

**Correct: D**

RAG retrieves the most current external documents at inference time, so updates to the knowledge source are reflected immediately without any retraining, which is ideal for fast-changing content.

**Why the others are wrong:**
- Fine-tuning weekly is costly, slow, and impractical for content that changes that frequently — it also risks the model still citing stale info between retrains
- Temperature controls randomness of wording, not factual accuracy or access to updated data
- Zero-shot prompting relies only on the model's frozen training data, which would not include this week's policy updates

> ⚠️ Frequently missed on the exam — read the options carefully.

</details>

---

**Q2.** A company wants a model that consistently writes marketing copy in a very specific brand voice and structure, regardless of the topic asked about. The style must be baked into the model's behavior, not just handled by instructions in each prompt. Which approach BEST meets this requirement?

A) Retrieval-Augmented Generation using the company's style guide as a knowledge source
B) Zero-shot prompting with no examples
C) Deploying an AI agent that calls external tools
D) Fine-tuning the model on many examples of brand-voice copy so the style becomes part of the model's learned behavior

<details>
<summary>Answer</summary>

**Correct: D**

Fine-tuning adapts the model's underlying behavior and style through additional training on examples, making the brand voice consistent across all future generations without needing it re-specified each time.

**Why the others are wrong:**
- RAG grounds facts in external data but does not reliably change the model's writing style or tone across all outputs
- Zero-shot prompting depends entirely on prompt wording each time and won't guarantee consistent style without reinforcement
- Agents orchestrate multi-step tool use; they don't inherently change writing style

> ⚠️ Frequently missed on the exam — read the options carefully.

</details>

---

**Q3.** A travel-booking assistant needs to check flight availability via one API, then check hotel availability via a second API, then combine both results into a single recommendation for the user — deciding which API to call and in what order based on the user's request. Which concept BEST describes this system?

A) A single-shot prompt with a large context window
B) A fine-tuned model with no external connections
C) A RAG pipeline querying only a static document store
D) An AI agent performing multi-step reasoning and tool use

<details>
<summary>Answer</summary>

**Correct: D**

An AI agent plans multi-step actions, decides which tools/APIs to invoke and in what order, and synthesizes results — exactly what's described here.

**Why the others are wrong:**
- A single-shot prompt cannot dynamically call external APIs or sequence actions
- A fine-tuned model alone has no built-in mechanism to call external tools or APIs
- A RAG pipeline retrieves from a document store; it does not orchestrate calls to multiple live APIs

</details>

---

**Q4.** Which technique is specifically used to reduce hallucinations by grounding a model's response in verified external or private data at query time?

A) Fine-tuning
B) Zero-shot prompting
C) Retrieval-Augmented Generation (RAG)
D) Increasing model temperature

<details>
<summary>Answer</summary>

**Correct: C**

RAG retrieves relevant, factual source content and injects it into the prompt context, anchoring the response to real data and reducing fabricated answers.

**Why the others are wrong:**
- Fine-tuning changes behavior/style but does not guarantee access to current factual data at inference time
- Zero-shot prompting provides no extra grounding data at all, making hallucination more likely, not less
- Increasing temperature increases randomness/creativity, which typically increases hallucination risk

</details>

---

**Q5.** A prompt engineer includes two example question-and-answer pairs in the prompt before asking the model the actual question, so the model can infer the desired answer format. What is this prompting technique called?

A) Zero-shot prompting
B) Few-shot prompting
C) Fine-tuning
D) Retrieval-Augmented Generation

<details>
<summary>Answer</summary>

**Correct: B**

Few-shot prompting provides a small number of example input/output pairs directly in the prompt so the model can pattern-match the expected format, without any retraining.

**Why the others are wrong:**
- Zero-shot prompting gives no examples at all, only an instruction
- Fine-tuning requires actual retraining of model weights, not examples placed in a live prompt
- RAG concerns retrieving external documents for factual grounding, not demonstrating output format

</details>

---

**Q6.** An engineer notices the model frequently invents plausible-sounding but false facts when the temperature parameter is set high. Which configuration change would MOST directly reduce this type of hallucination risk?

A) Increase the temperature further to encourage creativity
B) Lower the temperature to make outputs more deterministic and focused
C) Remove all context from the prompt
D) Switch to a longer context window without changing any other setting

<details>
<summary>Answer</summary>

**Correct: B**

Lowering temperature reduces randomness in token selection, making the model favor higher-probability, more grounded completions and reducing fabricated content.

**Why the others are wrong:**
- Increasing temperature increases randomness, which increases the likelihood of hallucinated content
- Removing context removes grounding information the model needs, increasing hallucination risk
- A longer context window alone does not address the randomness causing hallucination; it only allows more input/output tokens

> ⚠️ Frequently missed on the exam — read the options carefully.

</details>

---

**Q7.** A prompt consists only of a direct instruction such as 'Summarize this article in three sentences,' with no examples provided. Which prompting technique is this?

A) Zero-shot prompting
B) Few-shot prompting
C) Chain-of-thought prompting
D) Fine-tuning

<details>
<summary>Answer</summary>

**Correct: A**

Zero-shot prompting relies solely on instructions and context with no example input/output pairs, asking the model to complete the task directly using its pretrained knowledge.

**Why the others are wrong:**
- Few-shot prompting requires including example input/output pairs, which are absent here
- Chain-of-thought prompting explicitly asks the model to show step-by-step reasoning, which isn't described here
- Fine-tuning is a training process, not a prompt structure

</details>

---

**Q8.** What is a hallucination in the context of a large language model?

A) A deliberate refusal by the model to answer a question
B) A confident, fluent response that is factually incorrect or fabricated, not grounded in real data
C) An error message returned when the model's context window is exceeded
D) A response that exactly quotes the model's training data

<details>
<summary>Answer</summary>

**Correct: B**

Hallucination refers to the model generating plausible-sounding but false or unverifiable information, often because it is predicting statistically likely text rather than verified fact.

**Why the others are wrong:**
- A refusal to answer is a safety/guardrail behavior, not a hallucination
- Exceeding a context window produces a technical/token-limit error, not a hallucination
- Exact quoting of training data is the opposite of hallucination — hallucination involves invented content

</details>

---

