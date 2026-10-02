# Chapter 5 Cheat Sheet: CNNs, RNNs, Transformers

## Architecture Family → Data Type
| Architecture | Best For | Core Mechanism | Exam Keyword Trigger |
|---|---|---|---|
| CNN | Images, spatial data | Convolution (learned filters) | "image", "photo", "visual defect" |
| RNN (incl. LSTM/GRU) | Sequential/time-ordered data | Hidden state passed across time steps | "sequence", "time series", "sensor stream" |
| Transformer | Sequential data w/ long-range context, text | Self-attention (Query/Key/Value) | "language model", "long document", "chatbot context" |

## Self-Attention Basics (Awareness Level)
- Each token generates a **Query**, **Key**, and **Value** vector.
- Attention weight = similarity between Query and Key (all pairs computed in parallel).
- Output = weighted sum of Value vectors.
- Advantage over RNN: no sequential bottleneck → captures long-range dependencies, trains faster on large data/hardware.

## CNN Key Idea
- Filters/kernels slide over input to detect local patterns (edges → shapes → objects) in successive layers.
- Lower layers detect simple features; deeper layers combine them into complex representations.

## RNN Key Idea
- Processes input one step at a time, carrying a hidden state forward.
- Weakness: vanishing/exploding gradients on long sequences → limited long-range memory (LSTM/GRU mitigate but don't eliminate this).

## When to Use Deep Learning vs Classical ML
| Factor | Favors Classical ML | Favors Deep Learning |
|---|---|---|
| Data size | Small dataset | Large labeled dataset |
| Data type | Structured/tabular | Unstructured (image, audio, text) |
| Interpretability | High priority | Lower priority (black box acceptable) |
| Compute budget | Limited | Available (GPU/TPU) |
| Feature engineering | Manual features work well | Automatic feature learning needed |

## Common Enterprise Use Cases
- **CNN:** defect detection, medical imaging, facial recognition.
- **RNN:** legacy time-series forecasting, early speech recognition.
- **Transformer:** chatbots, document summarization, translation, modern LLM-based assistants.

## Exam Traps
1. Choosing RNN for long text tasks instead of Transformer — RNNs struggle with long-range context; exam favors Transformer for "long document" or "context across conversation" scenarios.
2. Choosing DL for small, structured, tabular datasets — classical ML (trees/boosting) is usually the better, exam-preferred answer.
3. Confusing CNN's convolution with Transformer's self-attention — convolution = local spatial filters; attention = global token relationships.
4. Assuming DL is always "better" — exam tests judgment on when classical ML is the right call (small data, interpretability needs).
