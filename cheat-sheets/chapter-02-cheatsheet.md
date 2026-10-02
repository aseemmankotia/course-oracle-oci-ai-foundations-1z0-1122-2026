# Chapter 2 Cheat Sheet: Supervised & Unsupervised Learning

## Domain Weight
Intro to Machine Learning Foundations — **15%** of exam

## The One Question That Decides Everything
**Does the data have labels (known correct outputs)?**
- **Yes → Supervised learning** (regression or classification)
- **No → Unsupervised learning** (clustering)

## Supervised vs Unsupervised

| Aspect | Supervised | Unsupervised |
|---|---|---|
| Data | Labeled (input + known output) | Unlabeled (input only) |
| Goal | Predict a known target for new data | Discover hidden structure/patterns |
| Techniques | Regression, Classification | Clustering |
| Example | Predict house price, classify spam | Segment customers, group similar sensor readings |

## Regression vs Classification (both Supervised)

| Aspect | Regression | Classification |
|---|---|---|
| Output type | Continuous number | Discrete category/class |
| Example question | "Predict the exact price/amount" | "Predict which category/class" |
| Sample use case | Sales forecast, temperature prediction | Spam/not spam, default/no default, disease/no disease |

## Decision Flow (memorize this)
1. Are labels present in the training data?
   - No → **Clustering** (unsupervised)
   - Yes → go to step 2
2. Is the label a continuous number?
   - Yes → **Regression**
   - No (it's a category) → **Classification**

## Common Exam Gotchas
1. **"Grouping" ≠ automatically clustering.** If the groups are already known/labeled in the data, it's supervised classification, not unsupervised clustering.
2. **Numeric-looking labels can still be categories.** A 0/1 flag for fraud is a category (classification), not a continuous measure (regression).
3. **Absence of a target column = unsupervised.** If the scenario says "no predefined categories" or "no known outcome," it's clustering, even if the data looks similar to a classification scenario.

## Quick Reference Examples
- Predict exact sales figure → **Regression**
- Predict Yes/No, category, or class → **Classification**
- Find natural groups with no known labels → **Clustering**

## Exam Note
The exam frequently tests this domain via short scenarios — read carefully for two clues: (1) whether labels/outcomes are mentioned as already known, and (2) whether the requested output is a number or a category/group.
