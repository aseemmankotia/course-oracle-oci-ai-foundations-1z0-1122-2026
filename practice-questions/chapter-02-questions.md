## Chapter 2: Machine Learning Foundations Part 1: Supervised & Unsupervised Learning — Practice Questions

**Q1.** A retail company wants to predict the exact dollar amount of next month's sales for each store based on historical sales data. Which type of ML task is this?

A) Regression
B) Classification
C) Clustering
D) Reinforcement learning

<details>
<summary>Answer</summary>

**Correct: A**

The output is a continuous numeric value (a dollar amount), which is the defining trait of regression.

**Why the others are wrong:**
- Classification predicts discrete categories, not continuous dollar values.
- Clustering groups unlabeled data with no target output; here there's a known historical target (sales amount).
- Reinforcement learning involves an agent learning via rewards from actions, not a static labeled dataset.

</details>

---

**Q2.** A bank wants to determine whether a loan applicant will default or not default on a loan. Which ML approach fits this requirement?

A) Regression
B) Clustering
C) Dimensionality reduction
D) Classification

<details>
<summary>Answer</summary>

**Correct: D**

The output is one of two discrete categories (default / not default), which is classification.

**Why the others are wrong:**
- Regression predicts a continuous number, not a category like default/not default.
- Clustering is used on unlabeled data to find groups, not to predict a known outcome from labeled data.
- Dimensionality reduction reduces feature count and isn't a predictive task type tested here.

</details>

---

**Q3.** A dataset contains customer transactions with no predefined categories or target values. The goal is to discover natural groupings of similar customers. Which approach applies?

A) Supervised classification
B) Supervised regression
C) Unsupervised clustering
D) Labeled regression

<details>
<summary>Answer</summary>

**Correct: C**

No labels or target values exist, and the goal is to find natural groupings — this is the definition of unsupervised clustering.

**Why the others are wrong:**
- Supervised classification requires labeled category data, which is absent here.
- Supervised regression requires a known continuous target, which is absent here.
- 'Labeled regression' is not a valid ML paradigm; regression always requires labels by definition, contradicting the unlabeled scenario.

</details>

---

**Q4.** What distinguishes supervised learning from unsupervised learning?

A) Supervised learning trains on labeled data with known outputs; unsupervised learning finds patterns in unlabeled data without predefined outputs
B) Supervised uses neural networks, unsupervised uses decision trees
C) Supervised learning is always faster to train than unsupervised learning
D) Unsupervised learning always requires more compute resources than supervised learning

<details>
<summary>Answer</summary>

**Correct: A**

The core distinction tested on the exam is the presence (supervised) or absence (unsupervised) of labeled output data, not algorithm type or speed.

**Why the others are wrong:**
- Algorithm choice (neural networks vs decision trees) is independent of the supervised/unsupervised distinction.
- Training speed is not a defining characteristic and varies by dataset and algorithm.
- Compute requirements depend on data size and algorithm, not on the paradigm itself.

</details>

---

**Q5.** A company has historical email data labeled as 'spam' or 'not spam' and wants to build a model to classify new incoming emails. Which best describes this task?

A) Unsupervised clustering because emails are grouped
B) Supervised classification because labels exist and the output is a category
C) Supervised regression because email content varies continuously
D) Unsupervised anomaly detection because spam is rare

<details>
<summary>Answer</summary>

**Correct: B**

Labels (spam/not spam) exist for training, and the output is a discrete category — this is supervised classification.

**Why the others are wrong:**
- The presence of labeled categories, not just 'grouping' language, rules out unsupervised clustering — clustering requires unlabeled data.
- Regression predicts continuous numeric outputs, not category labels like spam/not spam.
- Spam rarity doesn't change the fact that labels are present; anomaly detection is a different technique and not indicated here.

> ⚠️ Frequently missed on the exam — read the options carefully.

</details>

---

**Q6.** A data science team has an unlabeled dataset of sensor readings and wants to identify groups of similar equipment behavior for maintenance planning, with no known categories defined in advance. Which paradigm and technique should they choose?

A) Supervised learning with regression
B) Supervised learning with classification
C) Supervised learning with labeled anomaly categories
D) Unsupervised learning with clustering

<details>
<summary>Answer</summary>

**Correct: D**

No labels exist and the goal is to discover natural groupings, which is exactly what unsupervised clustering is designed for.

**Why the others are wrong:**
- Regression requires a labeled continuous target, which does not exist in this unlabeled dataset.
- Classification requires predefined labeled categories, which the team explicitly does not have.
- There are no labeled anomaly categories provided, so supervised learning cannot be applied here.

</details>

---

**Q7.** A hospital has patient records with diagnosis outcomes (disease present or absent) already recorded for each patient and wants to predict diagnosis for new patients. What does the presence of these labeled outcomes indicate about the correct approach?

A) The problem must use unsupervised clustering because diagnosis is categorical
B) The problem is supervised learning because labeled outputs exist, and since outputs are categorical, regression is appropriate
C) The problem is unsupervised because there are multiple diagnosis categories
D) The problem is supervised learning because labeled outputs exist, and since outputs are categorical, classification is appropriate

<details>
<summary>Answer</summary>

**Correct: D**

Labeled outcomes indicate supervised learning, and since the outcome is a category (present/absent), classification is the correct technique.

**Why the others are wrong:**
- Clustering applies to unlabeled data; labeled diagnosis data disqualifies this option.
- Regression is used for continuous numeric outputs, not categorical present/absent labels.
- Having multiple categories does not make a problem unsupervised — the key factor is the presence of labels, which exists here.

> ⚠️ Frequently missed on the exam — read the options carefully.

</details>

---

**Q8.** Which of the following is a classic example of unsupervised learning?

A) Predicting house prices from square footage and location
B) Classifying emails as spam or not spam
C) Predicting whether a transaction is fraudulent based on labeled fraud/not-fraud data
D) Grouping customers into segments based on purchasing behavior without predefined segments

<details>
<summary>Answer</summary>

**Correct: D**

Grouping customers with no predefined segments and no labeled target is the classic unsupervised clustering use case.

**Why the others are wrong:**
- Predicting house prices uses labeled continuous data (price), making it supervised regression.
- Classifying spam uses labeled categorical data, making it supervised classification.
- Fraud detection here explicitly uses labeled fraud/not-fraud data, making it supervised classification, not unsupervised.

</details>

---

