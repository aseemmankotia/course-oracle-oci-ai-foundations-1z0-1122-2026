## Chapter 3 Cheat Sheet — RL, ML Workflow & Evaluation

### Reinforcement Learning Core Loop
| Component | Definition |
|---|---|
| Agent | The learner/decision-maker |
| Environment | The system the agent interacts with |
| State | Current situation observed by the agent |
| Action | A choice the agent makes |
| Reward | Numeric feedback signal after an action |
| Policy | Mapping from states to actions (the strategy) |
| Episode | One full interaction sequence, start to terminal state |

**Exam note:** Agent acts → Environment returns new state + reward → Agent updates policy. Reward ≠ Policy — a very common trap.

### Typical ML Workflow Order
1. Data Collection
2. Data Preparation (cleaning, feature prep, encoding, scaling)
3. Train/Test Split
4. Model Training
5. Evaluation
6. Inference / Deployment

**Exam note:** Inference is always last. Evaluation always happens on held-out test data AFTER training, never before.

### Train/Test Split
| Purpose | Detail |
|---|---|
| Why split | Estimate generalization to unseen data |
| Common split ratios | 70/30 or 80/20 (train/test) — conceptual defaults, not fixed exam numbers |
| Rule | Never train on test data — invalidates evaluation |

### Overfitting vs Underfitting
| Symptom | Training Accuracy | Test Accuracy | Cause |
|---|---|---|---|
| Overfitting | High | Low (big gap) | Model too complex, memorizes noise |
| Underfitting | Low | Low | Model too simple, misses patterns |

**Exam note:** Gap size between train/test scores is the tell. Big gap = overfitting. Both low = underfitting.

### Evaluation Metrics (Conceptual)
| Metric | Use Case Note |
|---|---|
| Accuracy | Simple, but misleading on imbalanced data |
| Precision/Recall | Better for imbalanced classes (e.g., fraud, rare disease) |
| Confusion Matrix concept | Breaks down correct vs incorrect predictions per class |

**Common mistake:** Choosing accuracy as 'best' metric for a heavily imbalanced dataset scenario — exam tests recognizing this trap.

### Feature Preparation Basics
- Handle missing values
- Encode categorical variables
- Scale/normalize numeric features
- Happens BEFORE training, AFTER data collection

**Exam note:** Feature preparation quality directly affects model performance — 'garbage in, garbage out.'
