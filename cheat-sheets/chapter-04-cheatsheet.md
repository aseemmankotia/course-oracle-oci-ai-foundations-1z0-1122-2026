## Chapter 4 Cheat Sheet: Neural Network Foundations

### Layer Types
| Layer | Role | Size Determined By |
|---|---|---|
| Input | Receives raw features | Number of input features |
| Hidden | Extracts/transforms patterns | Design choice (depth = number of hidden layers) |
| Output | Produces final prediction | Number of classes/predicted values |

**Exam note:** Weights connect neurons between layers; biases shift the weighted sum before activation. Both are adjusted during training via **backpropagation + gradient descent**, not layer count or activation type.

### Activation Functions
| Function | Formula | Output Range | Typical Use |
|---|---|---|---|
| Sigmoid | 1/(1+e⁻ˣ) | (0, 1) | Binary classification output |
| Tanh | (eˣ−e⁻ˣ)/(eˣ+e⁻ˣ) | (-1, 1) | Hidden layers (zero-centered) |
| ReLU | max(0, x) | [0, ∞) | Most common hidden-layer choice |
| Softmax | normalized exponentials | (0,1), sums to 1 | Multi-class output layer |

**Common mistake:** Confusing ReLU with Leaky ReLU — standard ReLU outputs exactly **0** for negative inputs, not a small scaled negative value.

**Exam note:** Without activation functions (or with only linear ones), a network — no matter how deep — collapses into a single linear function and cannot learn complex, non-linear patterns.

### Why Depth Helps
- Each hidden layer builds more abstract features from the previous layer's output (e.g., edges → shapes → objects).
- Deep networks can represent complex functions more efficiently (fewer total neurons) than a single very wide shallow layer.
- **Exam trap:** Depth is not about needing less data — deep networks typically need MORE data and compute than shallow/classical models.

### Deep Learning vs. Classical ML
| Factor | Classical ML | Deep Learning |
|---|---|---|
| Data type | Structured/tabular | Unstructured (image, text, audio, video) |
| Data volume needed | Small–medium | Large |
| Feature engineering | Manual | Automatic (learned) |
| Interpretability | Higher | Lower |
| Compute needs | Lower | Higher |

**Exam note:** A scenario with a small tabular dataset and a need for interpretability → classical ML. A scenario with millions of images/text records → deep learning.

### Quick Formula
Neuron output: **y = f(Σ(wᵢ·xᵢ) + b)**, where f = activation function, w = weights, b = bias.

### Top Gotchas
1. Weights/biases are adjusted during training — NOT the number of layers or activation function type.
2. Sigmoid → (0,1); Tanh → (-1,1); ReLU → [0,∞) — know these ranges exactly.
3. Deep learning is not always the 'better' choice — it depends on data volume, structure, and interpretability needs.
