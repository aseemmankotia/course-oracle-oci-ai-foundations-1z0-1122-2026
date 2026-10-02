## Chapter 3: Machine Learning Foundations Part 2: Reinforcement Learning, Workflow & Evaluation — Practice Questions

**Q1.** A robotics team trains a warehouse robot to pick items faster without dropping them. The robot receives +1 when it places an item correctly and -1 when it drops one, then adjusts its future picking strategy based on this signal. In reinforcement learning terms, what is the +1/-1 signal called?

A) The policy
B) The reward
C) The environment
D) The episode

<details>
<summary>Answer</summary>

**Correct: B**

The reward is the numeric feedback signal the agent receives after taking an action, used to reinforce or discourage that behavior.

**Why the others are wrong:**
- The policy is the strategy/mapping from states to actions, not the feedback signal itself.
- The environment is the system the agent interacts with (the warehouse), not the feedback value.
- An episode is a complete sequence of agent-environment interaction from start to end, not the numeric signal.

> ⚠️ Frequently missed on the exam — read the options carefully.

</details>

---

**Q2.** A team trains a model that achieves 99% accuracy on training data but only 62% accuracy on new, unseen data. What is the MOST likely cause?

A) Overfitting to noise and specific patterns in the training set
B) Underfitting due to a model that is too simple
C) The evaluation metric was chosen incorrectly
D) The reward function was misconfigured

<details>
<summary>Answer</summary>

**Correct: A**

A large gap between excellent training performance and poor test performance is the classic signature of overfitting — the model memorized training data instead of learning generalizable patterns.

**Why the others are wrong:**
- Underfitting produces poor performance on BOTH training and test data, not a large gap between them.
- Metric choice affects how performance is measured, but it does not explain why training and test scores diverge so sharply.
- Reward functions apply to reinforcement learning, not to this supervised training/test accuracy scenario.

> ⚠️ Frequently missed on the exam — read the options carefully.

</details>

---

**Q3.** A data science team is building their first ML pipeline. Which sequence correctly reflects the typical ML workflow from start to finish?

A) Model training, data collection, data preparation, evaluation, inference
B) Data preparation, model training, data collection, inference, evaluation
C) Data collection, data preparation, model training, evaluation, inference
D) Evaluation, data collection, model training, data preparation, inference

<details>
<summary>Answer</summary>

**Correct: C**

The standard workflow order is: collect raw data, prepare/clean and split it, train the model, evaluate its performance, then deploy it for inference on new data.

**Why the others are wrong:**
- Training cannot happen before data is collected and prepared — there would be nothing to train on.
- Data collection must precede preparation and training; this order is reversed.
- Evaluation must follow training, not precede data collection — you cannot evaluate a model that does not yet exist.

</details>

---

**Q4.** In a reinforcement learning system, which component defines the mapping an agent uses to decide which action to take given its current state?

A) The reward
B) The environment
C) The policy
D) The episode

<details>
<summary>Answer</summary>

**Correct: C**

The policy is the agent's strategy — a function (often learned) that maps observed states to actions.

**Why the others are wrong:**
- The reward is feedback received after an action, not the decision-making mapping.
- The environment is the external system the agent acts within, not the agent's decision logic.
- An episode is a run of interaction from start to terminal state, unrelated to the state-to-action mapping.

> ⚠️ Frequently missed on the exam — read the options carefully.

</details>

---

**Q5.** A model performs poorly on both the training set and the test set, achieving low accuracy on each. Which problem does this MOST likely indicate?

A) Overfitting because the model is too complex
B) A missing train/test split
C) An incorrectly labeled reward signal
D) Underfitting because the model is too simple to capture patterns

<details>
<summary>Answer</summary>

**Correct: D**

Underfitting occurs when a model is too simple to capture underlying patterns, producing poor performance on both training and test data.

**Why the others are wrong:**
- Overfitting produces strong training performance paired with weak test performance — the opposite of poor performance on both.
- A missing train/test split is a process error, not a cause of uniformly poor accuracy on both sets when a split clearly exists.
- Reward signals apply to reinforcement learning, not to this supervised model's accuracy problem.

</details>

---

**Q6.** Why is a dataset typically split into separate training and test sets before building a model?

A) To estimate how well the model will generalize to data it has not seen before
B) To reduce the total amount of data needed for the project
C) To speed up the reward calculation during reinforcement learning
D) To automatically remove overfitting from the model

<details>
<summary>Answer</summary>

**Correct: A**

Holding out a test set allows evaluation of the model on data it never saw during training, giving a realistic estimate of real-world generalization performance.

**Why the others are wrong:**
- Splitting data does not reduce the total data collected; it partitions existing data.
- Reward calculation is specific to reinforcement learning and unrelated to train/test splitting in supervised learning.
- A train/test split reveals overfitting by exposing the training/test performance gap, but it does not itself remove or fix overfitting.

</details>

---

**Q7.** A dataset for a fraud detection model contains 990 legitimate transactions and only 10 fraudulent ones. A model that always predicts 'legitimate' achieves 99% accuracy. Why is accuracy alone a poor evaluation metric here?

A) Accuracy hides the model's failure to correctly identify the minority (fraud) class
B) Accuracy cannot be computed on imbalanced datasets
C) Accuracy only applies to reinforcement learning problems
D) Accuracy requires a train/test split to be calculated at all

<details>
<summary>Answer</summary>

**Correct: A**

On imbalanced data, a high accuracy score can be achieved simply by predicting the majority class, masking poor performance on the class that actually matters (fraud), which is why additional metrics are needed.

**Why the others are wrong:**
- Accuracy can technically be computed on any classification dataset, including imbalanced ones — the issue is interpretation, not calculability.
- Accuracy is a general evaluation metric used broadly in supervised learning, not something restricted to reinforcement learning.
- Accuracy calculation does not require a train/test split conceptually; the split is a separate best practice for generalization estimation.

> ⚠️ Frequently missed on the exam — read the options carefully.

</details>

---

**Q8.** What is the primary purpose of the feature preparation step in the ML workflow?

A) To define the reward function for the agent
B) To transform raw data into a clean, usable format the model can learn from effectively
C) To calculate the final accuracy of the trained model
D) To deploy the model for real-time inference

<details>
<summary>Answer</summary>

**Correct: B**

Feature preparation (cleaning, encoding, scaling, handling missing values) converts raw data into a structured format suitable for model training.

**Why the others are wrong:**
- Reward functions belong to reinforcement learning, not the general supervised ML feature preparation step.
- Accuracy calculation happens during the evaluation step, which comes after training, not during feature preparation.
- Deployment/inference is the final workflow step, occurring long after feature preparation and training are complete.

</details>

---

