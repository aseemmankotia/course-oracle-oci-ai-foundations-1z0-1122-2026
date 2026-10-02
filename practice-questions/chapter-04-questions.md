## Chapter 4: Deep Learning Foundations Part 1: Neural Networks, Layers, Weights & Activation — Practice Questions

**Q1.** A company wants to build a model that classifies millions of labeled product images into categories, where accuracy on raw pixel data matters more than interpretability. Which approach is BEST suited?

A) Classical ML using hand-crafted features and logistic regression
B) A rule-based expert system with manually coded rules
C) A deep neural network (e.g., a CNN) trained directly on the images
D) Linear regression with a single hidden layer

<details>
<summary>Answer</summary>

**Correct: C**

Deep learning excels at unstructured data like images when large labeled datasets are available, automatically learning hierarchical features without manual engineering.

**Why the others are wrong:**
- Hand-crafted features require manual feature engineering that doesn't scale well to raw pixel data at this volume.
- Rule-based systems can't generalize across millions of varied images.
- Linear regression cannot model the non-linear patterns needed for image classification, regardless of a single hidden layer.

</details>

---

**Q2.** During training, a neural network's predictions are far from the actual values. Which component is directly adjusted to reduce this error?

A) The number of layers in the network
B) The number of neurons in the output layer
C) The weights and biases of the network
D) The type of activation function used

<details>
<summary>Answer</summary>

**Correct: C**

Backpropagation combined with gradient descent adjusts weights and biases to minimize the loss function during training.

**Why the others are wrong:**
- The number of layers is an architecture decision made before training, not adjusted during it.
- Output layer size is fixed by the problem (e.g., number of classes), not adjusted during training.
- The activation function type is a design choice, not something updated iteratively during training.

> ⚠️ Frequently missed on the exam — read the options carefully.

</details>

---

**Q3.** You need an activation function for the output layer of a binary classification network that produces a probability between 0 and 1. Which should you use?

A) ReLU
B) Tanh
C) Linear (identity)
D) Sigmoid

<details>
<summary>Answer</summary>

**Correct: D**

Sigmoid squashes any input into the range (0, 1), making it ideal for representing a probability in binary classification.

**Why the others are wrong:**
- ReLU outputs values from 0 to infinity, not bounded probabilities.
- Tanh outputs values in (-1, 1), not a valid probability range.
- Linear activation is unbounded and cannot represent a probability.

</details>

---

**Q4.** A hidden layer uses standard ReLU activation. What is the output when the input to a neuron is negative?

A) The input value, unchanged
B) 1
C) 0
D) A small negative value scaled by 0.01

<details>
<summary>Answer</summary>

**Correct: C**

Standard ReLU is defined as f(x) = max(0, x), so any negative input outputs exactly 0.

**Why the others are wrong:**
- Passing the input unchanged describes a linear/identity function, not ReLU.
- ReLU never outputs 1 for a negative input; it is not bounded above at 1.
- Scaling by 0.01 describes Leaky ReLU, a variant, not standard ReLU — a common exam trap.

> ⚠️ Frequently missed on the exam — read the options carefully.

</details>

---

**Q5.** What is the primary purpose of an activation function in a neural network?

A) To reduce the total number of layers needed
B) To permanently store the learned weights
C) To introduce non-linearity so the network can model complex patterns
D) To normalize input data before training begins

<details>
<summary>Answer</summary>

**Correct: C**

Activation functions introduce non-linearity, which allows networks to approximate complex, non-linear relationships in data.

**Why the others are wrong:**
- Activation functions do not affect layer count decisions.
- Weights are stored as network parameters, not by the activation function.
- Data normalization is a preprocessing step, unrelated to activation function purpose.

</details>

---

**Q6.** A team has a small tabular dataset of 500 rows with clear structured features and needs an interpretable model delivered quickly. Which approach is MOST appropriate?

A) A classical ML model such as a decision tree or logistic regression
B) A deep neural network with 20 hidden layers
C) A convolutional neural network
D) A transformer-based deep learning model

<details>
<summary>Answer</summary>

**Correct: A**

Classical ML models work well and are more interpretable on small, structured datasets, and don't require the large data volumes deep learning needs to outperform them.

**Why the others are wrong:**
- Deep networks need large datasets to train effectively and would likely overfit on only 500 rows.
- CNNs are designed for grid-like/image data, not structured tabular features.
- Transformer models require large data and compute, and are overkill and hard to interpret for this small dataset.

> ⚠️ Frequently missed on the exam — read the options carefully.

</details>

---

**Q7.** Why can deep neural networks (many hidden layers) typically represent complex patterns, such as image features, more efficiently than shallow networks with a single hidden layer?

A) Deep networks always require less training data than shallow networks
B) Deep networks eliminate the need for activation functions entirely
C) Deep networks learn hierarchical representations, combining simple features into complex ones layer by layer
D) Deep networks always use fewer total weights than shallow networks

<details>
<summary>Answer</summary>

**Correct: C**

Depth allows networks to build increasingly abstract representations (e.g., edges to shapes to objects), which is more parameter-efficient for complex data than a single wide layer.

**Why the others are wrong:**
- Deep networks generally need MORE data, not less, to train effectively.
- Activation functions are still required at every layer for non-linearity, regardless of depth.
- Deep networks do not always have fewer weights; efficiency is about representation, not parameter count guarantees.

</details>

---

**Q8.** In a fully connected neural network, which layer directly produces the final prediction?

A) The input layer
B) The output layer
C) A hidden layer
D) An 'activation layer' separate from the others

<details>
<summary>Answer</summary>

**Correct: B**

The output layer produces the final prediction, sized to match the number of classes or predicted values.

**Why the others are wrong:**
- The input layer only receives raw feature data; it does not produce predictions.
- Hidden layers transform data between input and output but do not produce the final result.
- There is no separate 'activation layer' — activation functions are applied within each layer, not as a distinct layer type.

</details>

---

