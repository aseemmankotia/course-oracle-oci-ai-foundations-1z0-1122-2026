## Chapter 1: AI Fundamentals: Concepts, Categories & Enterprise Use Cases — Practice Questions

**Q1.** A retail company wants a system that predicts next quarter's inventory needs based on historical sales, seasonality, and promotional calendars. Which AI task category BEST describes this use case?

A) Forecasting
B) Anomaly detection
C) Recommendation
D) Natural language processing

<details>
<summary>Answer</summary>

**Correct: A**

Forecasting uses historical time-series data to predict future numeric outcomes such as demand or inventory levels.

**Why the others are wrong:**
- Anomaly detection identifies unusual deviations from normal patterns, not future predictions.
- Recommendation matches items/users based on preferences, not time-series prediction.
- NLP processes and generates human language, unrelated to numeric demand prediction.

> ⚠️ Frequently missed on the exam — read the options carefully.

</details>

---

**Q2.** A bank monitors millions of daily transactions and flags a small percentage that deviate sharply from a customer's normal spending pattern for manual review. Which AI task category is this?

A) Anomaly detection
B) Forecasting
C) Speech recognition
D) Computer vision

<details>
<summary>Answer</summary>

**Correct: A**

Anomaly detection identifies data points that differ significantly from expected patterns, exactly matching fraud-flagging behavior.

**Why the others are wrong:**
- Forecasting predicts future values, not detecting current outliers.
- Speech recognition converts audio to text and is unrelated to transaction analysis.
- Computer vision processes image/video data, not transaction records.

</details>

---

**Q3.** An online streaming platform suggests movies to a user based on what similar users watched and rated highly. Which AI task category applies?

A) Anomaly detection
B) Forecasting
C) Language generation
D) Recommendation

<details>
<summary>Answer</summary>

**Correct: D**

Recommendation systems suggest items based on similarity in user behavior or preferences, which is the core described scenario.

**Why the others are wrong:**
- Anomaly detection would flag unusual viewing behavior, not suggest new content.
- Forecasting predicts future trends/values, not personalized item matching.
- Language generation produces text output, not item suggestions.

</details>

---

**Q4.** Which statement correctly distinguishes traditional rule-based software from an AI system?

A) Rule-based software learns patterns from data, while AI follows only fixed if-then logic written by developers.
B) AI systems learn patterns from data and can generalize to new inputs, while rule-based software strictly follows pre-programmed logic.
C) AI and rule-based software are functionally identical, differing only in programming language used.
D) Rule-based software requires more training data than AI systems to operate correctly.

<details>
<summary>Answer</summary>

**Correct: B**

AI systems, especially machine learning models, learn statistical patterns from data and generalize to unseen inputs, whereas rule-based systems execute explicitly coded logic without learning.

**Why the others are wrong:**
- This reverses the actual definitions of the two approaches.
- The two are fundamentally different in how they derive decisions, not just implementation language.
- Rule-based software requires no training data at all; it runs on hardcoded rules.

> ⚠️ Frequently missed on the exam — read the options carefully.

</details>

---

**Q5.** A hospital deploys a chatbot that can only answer questions about appointment scheduling using a fixed decision tree, and cannot perform any other task such as diagnosing symptoms or writing reports. This system is best classified as:

A) General AI (AGI)
B) Responsible AI
C) Narrow AI
D) Anomaly detection AI

<details>
<summary>Answer</summary>

**Correct: C**

Narrow AI (also called Weak AI) is designed and trained for a single, specific task and cannot generalize beyond that scope, matching the appointment-only chatbot.

**Why the others are wrong:**
- General AI (AGI) refers to hypothetical systems capable of performing any intellectual task a human can, which does not currently exist in production systems.
- Responsible AI is a governance framework/principle set, not a category of AI capability.
- Anomaly detection is a task type, not a description of the system's general capability scope.

> ⚠️ Frequently missed on the exam — read the options carefully.

</details>

---

**Q6.** A company's AI-driven resume screening tool consistently ranks candidates from certain universities lower, even after controlling for qualifications, due to patterns learned from historically skewed hiring data. Which Responsible AI principle is being violated?

A) Transparency
B) Accountability
C) Availability
D) Fairness

<details>
<summary>Answer</summary>

**Correct: D**

Fairness in Responsible AI addresses ensuring the model does not produce discriminatory or biased outcomes against particular groups, which is exactly the scenario described.

**Why the others are wrong:**
- Transparency concerns whether stakeholders can understand how the model makes decisions, not the outcome bias itself.
- Accountability concerns having clear ownership and responsibility for model outcomes, not the bias pattern directly.
- Availability is not a Responsible AI principle; it is an infrastructure/reliability concept.

> ⚠️ Frequently missed on the exam — read the options carefully.

</details>

---

**Q7.** A financial institution wants regulators and customers to be able to understand WHY a loan application AI model rejected a specific applicant. Which Responsible AI principle does this requirement directly address?

A) Bias mitigation
B) Forecasting accuracy
C) Data anonymization
D) Transparency

<details>
<summary>Answer</summary>

**Correct: D**

Transparency refers to the ability to explain and understand how and why an AI model reached a particular decision, directly matching the requirement for explainable rejections.

**Why the others are wrong:**
- Bias mitigation addresses reducing unfair discrimination, not explainability of individual decisions.
- Forecasting accuracy is a model performance metric, unrelated to explainability requirements.
- Data anonymization is a privacy practice, not related to explaining decision logic.

</details>

---

**Q8.** A company deploys a generative AI chatbot for customer support. The chatbot occasionally produces confident-sounding but factually incorrect answers not grounded in any real source. This is an example of which known AI limitation?

A) Hallucination
B) Overfitting
C) Anomaly detection failure
D) Underfitting

<details>
<summary>Answer</summary>

**Correct: A**

Hallucination refers to generative AI producing plausible-sounding but false or fabricated content not grounded in training data or facts, a well-known limitation tested on the exam.

**Why the others are wrong:**
- Overfitting refers to a model memorizing training data and performing poorly on new data, a training-quality issue, not fabricated outputs.
- Anomaly detection failure is unrelated; the chatbot is a language generation task, not anomaly detection.
- Underfitting refers to a model failing to capture patterns in training data, resulting in poor performance overall, not fabricated confident answers.

> ⚠️ Frequently missed on the exam — read the options carefully.

</details>

---

