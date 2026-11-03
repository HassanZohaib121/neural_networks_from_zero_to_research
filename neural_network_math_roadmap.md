# Math You Need to Build Neural Networks From Scratch

If your goal is to create neural networks from zero, learn the mathematics in a practical order rather than studying an entire mathematics degree first.

You do **not** need advanced mathematics to start building neural networks. You need a solid understanding of a few important topics:

- Linear algebra
- Calculus
- Probability and statistics
- Optimization
- Numerical computation

Since you're a developer, the fastest route is to learn each mathematical concept alongside its implementation in Python and NumPy.

Your goal should be to understand how a neural network performs a forward pass, calculates its error, computes gradients, and updates its weights — without using PyTorch or TensorFlow initially.

## 1. The mathematics roadmap

Learn these topics in this order. This is the minimum practical foundation for implementing a neural network from scratch.

### Stage 1 — Basic mathematics (1–2 days)

- Functions: `f(x)`
- Exponents and logarithms
- Summation notation: `Σ`
- Basic algebra
- Graphs and slopes

Understand what a mathematical function does and how to manipulate its inputs and outputs.

### Stage 2 — Linear algebra (3–5 days)

- Scalars, vectors, matrices, tensors
- Vector addition and multiplication
- Dot product
- Matrix multiplication
- Transpose
- Broadcasting and dimensions

This is how neural networks represent inputs, weights, biases, and layer computations.

### Stage 3 — Calculus (4–6 days)

- Limits and derivatives
- Partial derivatives
- Chain rule
- Gradients
- Jacobian matrices
- Computational graphs

Calculus explains how changing a weight affects the network's output and loss.

### Stage 4 — Probability and statistics (2–4 days)

- Probability distributions
- Mean and variance
- Conditional probability
- Bayes' theorem
- Expected value
- Maximum likelihood estimation

Useful for understanding uncertainty, classification, loss functions, and model evaluation.

### Stage 5 — Optimization (2–3 days)

- Loss functions
- Gradient descent
- Learning rate
- Stochastic gradient descent (SGD)
- Momentum
- Adam optimizer

Understand how the network learns by repeatedly adjusting its parameters to reduce errors.

These are focused learning estimates, not full university courses. You can begin coding before mastering every topic.

## 2. Best resources — in the order recommended

You don't need ten courses. These five resources are enough to get started.

### 1. 3Blue1Brown — Essence of Linear Algebra

Learn vectors, matrices, dot products, and transformations visually.

- [Watch the series](https://www.3blue1brown.com/topics/linear-algebra)
- Free

### 2. 3Blue1Brown — Essence of Calculus

Learn derivatives, the chain rule, and the intuition behind gradients.

- [Watch the series](https://www.3blue1brown.com/topics/calculus)
- Free

### 3. Andrej Karpathy — Neural Networks: Zero to Hero

A top recommendation. Build backpropagation, an MLP, and eventually GPT. You learn the math while coding.

- [Course and lectures](https://karpathy.ai/zero-to-hero.html)
- [Micrograd lecture](https://www.youtube.com/watch?v=VMj-3S1tku0)
- Free

### 4. Neural Networks and Deep Learning — Michael Nielsen

A free online book that explains neural networks, gradient descent, and backpropagation in detail.

- [Read the book](http://neuralnetworksanddeeplearning.com/)
- Free

### 5. Mathematics for Machine Learning

A more formal reference for linear algebra, calculus, probability, and optimization.

- [Free book and resources](https://mml-book.github.io/)
- Optional deeper study

The first three resources are the most important for your immediate goal.

## 3. The most important mathematical concepts, with examples

Here are the concepts you should actually understand, not just memorize.

### A. Linear algebra: the forward pass

A neuron computes:

\[
z = w_1x_1+w_2x_2+b
\]

Then an activation function is applied:

\[
a = \sigma(z)
\]

For a whole layer, this becomes:

\[
a = \sigma(Wx+b)
\]

You should understand:

- Why weights are multiplied by inputs.
- Why we add a bias.
- Why matrices allow us to calculate many neurons together.
- How to determine the dimensions of `W`, `x`, and `b`.

### B. Calculus: how a network learns

Suppose the network has a loss function:

\[
L(w)=(wx-y)^2
\]

The derivative tells us how the loss changes when the weight changes:

\[
\frac{dL}{dw}=2x(wx-y)
\]

This is the foundation of learning.

The network adjusts its weights using:

\[
w_{\text{new}}=w_{\text{old}}-\eta\frac{dL}{dw}
\]

Here, `η` is the learning rate.

### C. Chain rule: the heart of backpropagation

Consider a simple network:

\[
x \rightarrow z \rightarrow a \rightarrow L
\]

The chain rule tells us:

\[
\frac{dL}{dx}
=
\frac{dL}{da}
\frac{da}{dz}
\frac{dz}{dx}
\]

Backpropagation is essentially the systematic application of the chain rule throughout a computational graph.

**If you understand the chain rule deeply, you understand the central mathematical idea behind neural network training.**

### D. Probability: classification

For a classification network, you will need to understand softmax:

\[
P(y=i)=
\frac{e^{z_i}}{\sum_j e^{z_j}}
\]

And cross-entropy loss:

\[
L=-\sum_i y_i\log(p_i)
\]

This combination is commonly used to train classification models.

## 4. Your fastest 14-day learning plan

Assuming you can spend 2–3 hours daily:

| Day | Study | Practical goal |
|---|---|---|
| 1 | Functions, algebra, exponents | Implement basic functions in Python |
| 2 | Vectors and dot products | Implement a neuron |
| 3 | Matrices and matrix multiplication | Implement a dense layer |
| 4 | Derivatives and slopes | Calculate derivatives manually |
| 5 | Partial derivatives and gradients | Calculate gradients for multiple weights |
| 6 | Chain rule | Derive a simple computational graph |
| 7 | Review calculus and linear algebra | Build a single-neuron model |
| 8 | Loss functions | Implement MSE loss |
| 9 | Gradient descent | Train a linear regression model |
| 10 | Backpropagation | Implement a 2-layer network |
| 11 | Activations: ReLU, sigmoid, tanh | Implement activation functions |
| 12 | Softmax and cross-entropy | Build a classification network |
| 13 | Probability and initialization | Train a small neural network |
| 14 | Complete project | Train a neural network using NumPy only |

You don't need to complete every advanced topic in 14 days. This is a practical starting schedule.

## 5. What you should build from scratch

This is the project sequence recommended.

### Project 1: Single Neuron

Implement:

- Inputs, weights, and bias
- Forward pass
- MSE loss
- Derivative
- Gradient descent

### Project 2: Neural Network with 2 Layers

Implement:

- Multiple neurons
- Hidden layer
- ReLU or sigmoid
- Backpropagation
- Weight updates

### Project 3: MNIST Digit Classifier

Implement:

- Input layer: 784 neurons
- Hidden layer: 128 neurons
- Output layer: 10 neurons
- Softmax
- Cross-entropy loss
- Mini-batch gradient descent

### Project 4: Build a Tiny GPT

Once the above is understood, explore:

- Embeddings
- Attention
- Positional encoding
- Transformer blocks
- Layer normalization
- Autoregressive training

## 6. What NOT to study initially

Don't waste your initial time on these:

- Eigenvalues and eigenvectors in depth
- Advanced integration techniques
- Differential equations
- Measure theory
- Advanced statistical inference
- Tensor calculus in full generality
- Proof-heavy mathematics

These topics may become useful later, but they are not prerequisites for building your first neural network.

## 7. Recommended learning sequence

Follow this exact sequence:

1. Watch the first 4–5 videos of 3Blue1Brown's linear algebra series.
2. Watch the first 5–6 videos of the calculus series, focusing on derivatives and the chain rule.
3. Start Karpathy's Zero to Hero course, Lecture 1: build `micrograd`.
4. Implement the same neural network yourself using Python and NumPy, without copying the entire implementation.
5. Continue to the MLP and manually implement its backpropagation.
6. Build a tiny GPT only after you understand the previous steps.

Karpathy's course is especially relevant because it progresses from scalar-level automatic differentiation to neural networks and GPT, with a dedicated lecture on manually implementing backpropagation.

## Final recommendation

**The single best starting point:** [Karpathy's micrograd lecture](https://www.youtube.com/watch?v=VMj-3S1tku0).

You can begin it with only basic Python and a vague recollection of high-school calculus.

Remember: don't just watch the videos. Pause, solve the examples yourself, implement the equations, and experiment with changing weights and learning rates. The goal is to understand every operation well enough to implement it without a machine-learning framework.
