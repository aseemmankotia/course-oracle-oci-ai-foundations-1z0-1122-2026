# Chapter 7 Cheat Sheet: Prompt Engineering, RAG, Fine-Tuning & Agents

## RAG vs Fine-Tuning vs Prompt Engineering
| Technique | Changes | Best For | Retraining Needed? |
|---|---|---|---|
| Prompt Engineering | Nothing in the model — only the input | Quick, low-cost behavior steering per request | No |
| RAG | Adds external/private data at query time | Fast-changing facts, private/proprietary knowledge, reducing hallucinations | No |
| Fine-Tuning | Model's weights/learned behavior | Consistent style, tone, domain jargon, task specialization | Yes |

**Exam rule of thumb:** "needs the latest/private data" → RAG. "needs consistent style/behavior every time" → Fine-tuning. "needs quick one-off formatting" → Prompt engineering.

## Prompting Techniques
| Technique | Examples in Prompt? | Use Case |
|---|---|---|
| Zero-shot | No | Simple, general tasks the model already knows well |
| Few-shot | Yes (a handful) | Teaching a specific output format/pattern |
| Chain-of-thought | No (but asks for reasoning steps) | Multi-step logic, math, complex reasoning |

**Prompt = Instructions + Examples (optional) + Context**

## RAG Pipeline (3 Steps)
1. **Retrieve** — embed query, search vector DB for similar chunks
2. **Augment** — inject retrieved chunks into the prompt
3. **Generate** — LLM produces a grounded response

## AI Agents
- Definition: LLM-driven system that performs **multi-step reasoning** and **tool/API use** to achieve a goal (not just single-turn text generation).
- Loop pattern: **Plan → Act (call tool) → Observe result → Repeat → Final answer.**
- Exam trap: A system that only answers from a single prompt with no tool calls is NOT an agent, even if it uses RAG.

## Hallucinations
- **Definition:** confident, fluent, but false/fabricated output.
- **Causes:** no grounding data, ambiguous/underspecified prompts, high temperature, gaps in training data.
- **Mitigations:** RAG grounding, lower temperature, clearer prompts/context, human review for high-stakes use.

## Temperature Quick Reference
| Setting | Behavior | Hallucination Risk |
|---|---|---|
| Low (e.g., 0–0.3) | Deterministic, focused | Lower |
| High (e.g., 0.7–1.0+) | Creative, varied | Higher |

## Responsible Generative AI Checklist
- Disclose AI-generated content (**transparency**)
- Check for and mitigate **bias/fairness** issues
- Maintain **human accountability** for AI-assisted decisions
- Protect **privacy** of data used in prompts/training
- Validate outputs before high-stakes use to catch **hallucinations**

### Common Exam Traps
1. Choosing fine-tuning when the requirement is really about fresh/changing facts (should be RAG).
2. Confusing few-shot (has examples) with zero-shot (no examples).
3. Thinking RAG changes the model's tone/style — it only grounds facts, it does not alter behavior/style like fine-tuning does.
