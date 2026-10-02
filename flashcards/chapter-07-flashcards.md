## Chapter 7: Generative AI & LLMs Part 2: Prompt Engineering, RAG, Fine-Tuning & Agents — Flashcards

| # | Front (Question) | Back (Answer) |
|---|-----------------|---------------|
| 1 | RAG vs Fine-tuning: which one updates a model's factual knowledge WITHOUT retraining? | RAG. It retrieves current external/private data at query time. Fine-tuning instead changes the model's learned behavior/style through additional training — use it for tone, format, or domain-specific behavior, not fast-changing facts. |
| 2 | When should you choose Fine-tuning over RAG? | When you need to change the model's STYLE, TONE, or BEHAVIOR consistently (e.g., brand voice, specialized jargon) rather than inject fresh factual data. Exam tip: 'consistent style/behavior' = fine-tuning; 'current/private facts' = RAG. |
| 3 | Zero-shot prompting — definition? | Giving the model only an instruction/context, no examples, and expecting it to complete the task using pretrained knowledge alone. |
| 4 | Few-shot prompting — definition? | Including a small number of example input/output pairs in the prompt so the model can infer the desired format or pattern before answering the real question. |
| 5 | Chain-of-thought prompting — definition? | A prompting technique that instructs the model to reason step-by-step before giving a final answer, improving performance on multi-step logic/math tasks. |
| 6 | Three core components of a well-engineered prompt? | Instructions (what to do), Examples (how to do it — optional, used in few-shot), Context (background info needed to answer correctly). |
| 7 | Basic RAG pipeline steps (in order)? | 1) Retrieve relevant documents/chunks from a knowledge base (often via vector embeddings), 2) Augment the prompt with retrieved content, 3) Generate the response grounded in that content. |
| 8 | What powers the 'retrieval' step in RAG? | Typically a vector database storing embeddings of documents; the user query is embedded and matched to the most semantically similar chunks, which are then passed to the LLM as context. |
| 9 | AI agent — core conceptual definition? | A system that uses an LLM to perform multi-step reasoning, decide which tools/APIs to call, execute those actions, and combine results to accomplish a goal — beyond single-turn text generation. |
| 10 | Main cause of LLM hallucinations? | The model generates the statistically most probable next tokens, not verified facts. Lack of grounding data, ambiguous prompts, and high temperature settings all increase hallucination risk. |
| 11 | Temperature parameter — effect on output? | Controls randomness of token selection (typical range ~0.0–1.0+ depending on platform). Lower = more deterministic/focused, reduces hallucination risk. Higher = more creative/varied, increases hallucination risk. Exam tip: lower temperature for factual/precise tasks. |
| 12 | Key responsible generative AI considerations tested on the exam? | Transparency (disclose AI-generated content), fairness/bias mitigation, accountability for outputs, privacy of training/input data, and mitigating hallucinations before deploying AI in high-stakes decisions. |
