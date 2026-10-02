## Chapter 3: Machine Learning Foundations Part 2: Reinforcement Learning, Workflow & Evaluation — Flashcards

| # | Front (Question) | Back (Answer) |
|---|-----------------|---------------|
| 1 | In reinforcement learning, what are the four core components of the agent-environment loop? | Agent, Environment, Action, Reward (plus State). Exam tip: the agent takes an action in the environment, receives a reward and a new state, then updates its policy. |
| 2 | What is a 'policy' in reinforcement learning? | The strategy/function mapping states to actions. Exam tip: don't confuse policy (decision rule) with reward (feedback signal). |
| 3 | What is the correct high-level ML workflow order? | Data collection → Data preparation → Model training → Evaluation → Inference/Deployment. Exam tip: questions often scramble this order — inference is always last. |
| 4 | Why split data into train and test sets? | To estimate how well the model generalizes to unseen data. Exam tip: the test set must NOT be used during training or it invalidates the evaluation. |
| 5 | Overfitting vs Underfitting — how to tell them apart? | Overfitting: high training accuracy, low test accuracy (big gap). Underfitting: low accuracy on BOTH sets. Exam tip: gap size is the key differentiator. |
| 6 | What causes underfitting? | A model that is too simple to capture underlying patterns in the data. Exam tip: the fix is a more complex/expressive model or better features, not more data alone. |
| 7 | What causes overfitting? | A model that is too complex and learns noise/specifics of the training data rather than general patterns. Exam tip: the fix conceptually includes more training data, simpler models, or regularization. |
| 8 | Why is accuracy alone often misleading on imbalanced datasets? | A model can achieve high accuracy by always predicting the majority class while completely failing on the minority class. Exam tip: fraud/rare-event detection scenarios test this concept. |
| 9 | What is 'feature preparation' in the ML workflow? | Cleaning, transforming, and structuring raw data (handling missing values, encoding, scaling) before training. Exam tip: happens right after data collection, before model training. |
| 10 | Reinforcement Learning vs Supervised Learning — key difference? | Supervised learning learns from labeled examples; reinforcement learning learns through trial-and-error via rewards from interacting with an environment. Exam tip: RL has no fixed labeled dataset upfront. |
| 11 | What is an 'episode' in reinforcement learning? | One complete sequence of agent-environment interaction from an initial state to a terminal state. Exam tip: distinguish episode (a full run) from a single action/step. |
| 12 | What does 'evaluation' accomplish in the ML workflow, and where does it sit? | It measures trained model performance (e.g., accuracy) using held-out test data; it occurs after training and before deployment/inference. Exam tip: evaluation results decide whether the model is ready for inference. |
