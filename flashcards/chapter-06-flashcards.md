## Chapter 6: Generative AI & LLMs Part 1: Generative vs Discriminative, Tokens, Embeddings & Context — Flashcards

| # | Front (Question) | Back (Answer) |
|---|-----------------|---------------|
| 1 | Generative AI — core definition? | AI that creates NEW content (text, images, audio, code) rather than just predicting a label or score. Exam tip: if the question says 'creates something new' → generative; if it says 'classifies/predicts' → discriminative. |
| 2 | Discriminative (predictive) model — what does it learn? | Learns to distinguish between classes / predict a label given input (models P(label \| input)). Used for classification, regression, spam detection. |
| 3 | Generative model — what does it learn? | Learns the underlying data distribution so it can generate new, similar samples (e.g., new text, images). Contrast with discriminative models which only separate classes. |
| 4 | What is a 'token' in an LLM? | A unit of text — a word, subword, or character sequence — that the tokenizer converts to a numeric ID. LLMs process and generate one token at a time. |
| 5 | Rough token-to-text ratio (English)? | ≈ 1 token per 4 characters, or roughly 0.75 words per token, as a general estimate. Exam tip: used to reason about how much text fits in a context window, not an exact/official conversion. |
| 6 | How does an LLM generate text step-by-step? | Autoregressively: it computes a probability distribution over the entire vocabulary for the NEXT token, conditioned on all prior tokens, then selects/samples one token and repeats. |
| 7 | What is an embedding? | A numerical vector representation of text (or other data) that captures semantic meaning — similar meanings produce vectors that are close together in vector space. |
| 8 | Why use embeddings instead of raw text for similarity search? | Embeddings let you compare MEANING, not exact wording — e.g. 'reset password' and 'can't log in' can have close vectors even though the words differ. |
| 9 | What is a context window? | The maximum number of tokens (prompt + generated response combined) a model can process/consider at one time. Exceeding it causes truncation or an error. |
| 10 | What happens if input + expected output exceeds the context window? | Input gets truncated, the request may be rejected, or earlier content is dropped from consideration — the model cannot 'expand' its window on the fly. |
| 11 | Generative vs Discriminative — quick memory trick? | Generative = 'Generates' new stuff. Discriminative = 'Discriminates' (decides) between existing categories/labels. |
| 12 | Common exam trap: is classification considered generative AI? | No — classification (assigning a label from a fixed set) is a discriminative/predictive task, even if performed by a large neural network. Generative AI must produce new content. |
