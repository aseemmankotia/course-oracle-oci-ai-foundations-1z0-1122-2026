## AI Foundations Cheat Sheet (Domain Weight: 10%)

### AI vs Traditional Software
| Aspect | Rule-Based Software | AI System |
|---|---|---|
| Logic source | Hardcoded if-then rules | Learned patterns from data |
| Adapts to new data? | No | Yes (generalizes) |
| Example | Tax bracket calculator | Spam filter trained on emails |

### Narrow AI vs General AI (AGI)
| | Narrow AI | General AI (AGI) |
|---|---|---|
| Scope | Single specific task | Any human-level task |
| Exists today? | Yes — all deployed AI | No — theoretical/future |
| Example | Image classifier, chatbot | N/A (hypothetical) |

### Core AI Task Categories
| Task Type | What It Does | Enterprise Example |
|---|---|---|
| Language (NLP) | Process/generate text | Chatbots, sentiment analysis |
| Vision | Interpret images/video | Defect detection, OCR |
| Speech | Convert audio↔text | Call transcription, IVR |
| Recommendation | Suggest items via similarity | 'Customers also bought' |
| Anomaly Detection | Flag outliers vs normal pattern | Fraud detection |
| Forecasting | Predict future numeric values | Demand/inventory prediction |

**Exam keyword mapping:**
- 'unusual/outlier/fraud' → Anomaly Detection
- 'predict future/next quarter/trend' → Forecasting
- 'suggest/similar users' → Recommendation
- 'text/chat/translate' → Language
- 'image/photo/video' → Vision
- 'audio/voice/transcribe' → Speech

### Responsible AI Principles
| Principle | Focus | Violation Example |
|---|---|---|
| Bias | Skewed patterns from data | Model trained on unbalanced historical data |
| Fairness | Equitable outcomes across groups | Resume screener ranks certain groups lower |
| Transparency | Explainability of decisions | Black-box loan rejection with no reason given |
| Accountability | Clear ownership of AI impact | No one responsible when model causes harm |

### AI Risks & Limitations
| Term | Meaning | Common Confusion |
|---|---|---|
| Hallucination | Confident but false generated output | NOT the same as overfitting |
| Overfitting | Memorizes training data, fails on new data | Training-quality issue |
| Underfitting | Fails to capture patterns even in training | Model too simple |
| Bias amplification | Model magnifies existing data bias | Distinct from random error |

### Common Exam Traps
1. Confusing 'bias' (the problem) with 'fairness' (the goal principle) — question asks which PRINCIPLE is violated, not just naming the flaw.
2. Selecting 'General AI' for any advanced-sounding narrow system — AGI does not exist in production; if it's deployed and doing one job, it's Narrow AI.
3. Mixing up hallucination (generative AI fabrication) with overfitting (training data memorization) — different root causes, different fixes.
