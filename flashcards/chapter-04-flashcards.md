## Chapter 4: Deep Learning Foundations Part 1: Neural Networks, Layers, Weights & Activation — Flashcards

| # | Front (Question) | Back (Answer) |
|---|-----------------|---------------|
| 1 | What are the three types of layers in a basic neural network? | Input, Hidden, and Output. Exam tip: input layer size = number of features; output layer size = number of classes/predicted values. |
| 2 | What does a 'weight' represent in a neural network? | The strength/importance of the connection between two neurons. Exam tip: weights (and biases) are the parameters adjusted during training via backpropagation. |
| 3 | Sigmoid activation function — output range? | (0, 1). Exam tip: commonly used in the output layer for binary classification to represent a probability. |
| 4 | Tanh activation function — output range? | (-1, 1). Exam tip: zero-centered, often preferred over sigmoid in hidden layers for faster convergence. |
| 5 | ReLU formula and output for negative input? | ReLU(x) = max(0, x); outputs exactly 0 for any negative input. Exam tip: most common hidden-layer activation, helps avoid vanishing gradients. |
| 6 | What algorithm adjusts weights based on prediction error? | Backpropagation combined with gradient descent. Exam tip: error from the loss function is propagated backward to update weights layer by layer. |
| 7 | Why do deep networks outperform shallow ones on complex data like images? | They learn hierarchical features — early layers detect edges, later layers combine them into shapes/objects. Exam tip: depth enables efficient representation of complex functions. |
| 8 | When is classical ML preferred over deep learning? | Small or structured (tabular) datasets, need for interpretability, limited compute/data. Exam tip: deep learning needs large datasets/compute to outperform classical ML. |
| 9 | When is deep learning preferred over classical ML? | Large volumes of unstructured data — images, text, audio, video. Exam tip: DL automatically learns features, removing the need for manual feature engineering. |
| 10 | What is a neuron's basic computation? | Weighted sum of inputs plus bias, passed through an activation function: y = f(Σ(wᵢxᵢ) + b). Exam tip: know the difference between 'weight' and 'bias' terms. |
| 11 | What happens if a network uses only linear activation functions (or none)? | The entire network collapses into a single linear function regardless of depth, and cannot model non-linear patterns. Exam tip: this is why activation functions are essential. |
| 12 | What determines the output layer's size? | The number of predicted classes/values — e.g., 1 neuron for binary classification, N neurons for N-class classification. Exam tip: multi-class output layers are typically paired with softmax activation. |
