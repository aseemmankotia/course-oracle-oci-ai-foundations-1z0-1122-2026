## Chapter 6 Cheat Sheet: Generative vs Discriminative, Tokens, Embeddings & Context

### Generative vs Discriminative Models
| Aspect | Generative Model | Discriminative Model |
|---|---|---|
| Goal | Create new content | Predict/classify a label |
| Learns | Data distribution (how data is produced) | Decision boundary between classes |
| Output example | New text, image, code | Category, score, label |
| Example task | Write an email, generate an image | Spam vs not-spam, sentiment score |
| Memory trick | 'Generates' new stuff | 'Discriminates' between labels |

**Exam note:** If a scenario says the system must *produce/create* something new → generative. If it must *sort/label/predict* from a fixed set of outcomes → discriminative.

### Tokens & Tokenization
- A **token** = smallest unit an LLM processes (word, subword, or character chunk) mapped to a numeric ID.
- Rough estimate: **~1 token ≈ 4 characters** or **~0.75 words** in English (approximation only — not an exact/official ratio).
- Tokenization happens BEFORE the model sees text; the model never sees raw characters, only token IDs.

**Common mistake:** Assuming 1 token = 1 word always. Subwords and punctuation can each be separate tokens, so token counts are usually HIGHER than word counts.

### How LLMs Generate Text (Autoregressive Generation)
1. Model receives tokens so far (prompt + generated tokens).
2. Computes a probability distribution over the ENTIRE vocabulary for the next token.
3. Selects/samples one token (greedy, top-k, or temperature-based sampling).
4. Appends token, repeats until stop condition (max tokens or end-of-sequence).

**Exam note:** This token-by-token, conditioned-on-prior-tokens process is called **autoregressive generation**.

### Embeddings
- **Definition:** A dense numeric vector representing the *meaning* of text (or other data).
- Similar meaning → vectors close together in vector space (measured via cosine similarity or similar metrics).
- Used for: semantic search, clustering, retrieval-augmented generation (RAG), recommendation.

**Common mistake:** Confusing embeddings (meaning representation, used for similarity/retrieval) with tokens (raw text units used for generation input/output).

### Context Window
- **Definition:** Maximum number of tokens (prompt + response combined) the model can process in a single request.
- It is FIXED per model/deployment — it does not expand dynamically.
- Exceeding the limit → truncation, dropped content, or request error.

**Exam note:** Longer conversations or documents may need chunking, summarization, or retrieval strategies (like RAG) to stay within the context window rather than expecting the model to 'remember' unlimited history.

### Quick Recap Table
| Concept | One-liner |
|---|---|
| Generative AI | Creates new content |
| Discriminative model | Predicts/classifies existing input |
| Token | Unit of text the model reads/writes |
| Embedding | Vector capturing semantic meaning |
| Context window | Max tokens model can handle at once |
| Autoregressive generation | Predicts next token from prior tokens, one at a time |
