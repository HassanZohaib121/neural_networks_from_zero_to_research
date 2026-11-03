# Neural Networks From Zero to Research
## Personalized 12-Month Learning Course

**Starting level**
- Python: No prior experience
- Mathematics: School-level mathematics
- Ultimate goal: Understand neural networks deeply, read research papers, reproduce experiments, and eventually conduct independent research.

**Recommended study time:** 2–3 hours per day, six days per week.

> This is an ambitious foundation-building plan, not a guarantee of research expertise in 12 months. Independent research usually requires continued study and experimentation beyond this course.

---

## 1. Course overview

The course has six stages:

| Stage | Duration | Main subject |
|---|---:|---|
| 1 | Months 1–2 | Mathematics and Python foundations |
| 2 | Months 3–4 | Advanced mathematics and machine learning |
| 3 | Months 5–6 | Neural networks from scratch |
| 4 | Months 7–8 | Deep learning architectures |
| 5 | Months 9–10 | Advanced deep learning and research mathematics |
| 6 | Months 11–12 | Research papers and independent experiments |

### Learning philosophy

- Understand concepts before memorizing formulas.
- Derive equations instead of blindly applying them.
- Implement algorithms before relying on libraries.
- Visualize mathematical operations and training behavior.
- Test implementations against known results.
- Read research papers and reproduce experiments.

---

# Stage 1 — Foundations (Months 1–2)

The first objective is to become comfortable with programming and mathematical reasoning.

## Module 1: Mathematics for computer science

**Duration:** 3 weeks

### Lessons
1. Numbers and number systems
2. Fractions and decimals
3. Percentages and ratios
4. Algebraic expressions
5. Equations and inequalities
6. Functions and graphs
7. Exponents and logarithms
8. Summation notation
9. Coordinate geometry
10. Basic trigonometry

### Why it matters

Neural networks are mathematical functions. You need to understand how inputs are transformed into outputs.

For example:

\[
f(x)=2x+3
\]

If \(x=4\), then:

\[
f(4)=2(4)+3=11
\]

Eventually, you will understand neural networks as compositions of many functions.

### Exercises
- Solve 30 algebraic equations.
- Draw graphs of 10 mathematical functions.
- Calculate logarithms and exponents.
- Write Python programs that evaluate mathematical functions.

## Module 2: Python programming from zero

**Duration:** 4 weeks

### Weekly lessons

| Week | Topics |
|---|---|
| 1 | Variables, data types, operators, input/output |
| 2 | Conditions, loops, functions |
| 3 | Lists, tuples, dictionaries, sets |
| 4 | Classes, objects, modules, exceptions, files |

### Additional topics
- Function arguments, return values, and scope
- List comprehensions
- Lambda functions
- Iterators and generators
- Object-oriented programming
- Debugging and testing
- Virtual environments and packages

### Projects
1. Calculator
2. Number guessing game
3. Student marks management system
4. Scientific calculator
5. Mathematical function plotter

## Module 3: Python for scientific computing

**Duration:** 1 week

### Learn
- NumPy arrays
- Array dimensions and shapes
- Matrix operations
- Broadcasting
- Matplotlib plotting
- Jupyter Notebook

### Project
Build a small mathematical computing environment using Python and NumPy.

---

# Stage 2 — Mathematics and Machine Learning (Months 3–4)

This stage is especially important for research ambitions.

## Module 4: Linear algebra

**Duration:** 3 weeks

### Lessons
1. Scalars and vectors
2. Vector addition and subtraction
3. Dot products
4. Matrix representation
5. Matrix addition and multiplication
6. Matrix transpose
7. Identity matrices
8. Inverse matrices
9. Linear transformations
10. Eigenvalues and eigenvectors

A foundational neural-network operation is:

\[
y=Wx+b
\]

Understand what this equation means geometrically and computationally.

### Exercises
- Multiply matrices manually.
- Implement matrix multiplication in Python.
- Implement dot products without NumPy.
- Visualize vector transformations.

## Module 5: Calculus

**Duration:** 3 weeks

### Lessons
1. Functions and limits
2. Continuity
3. Derivatives
4. Power rule
5. Product rule
6. Quotient rule
7. Chain rule
8. Partial derivatives
9. Multivariable functions
10. Gradients

The chain rule is especially important:

\[
\frac{dy}{dx}=\frac{dy}{du}\frac{du}{dx}
\]

It is one of the mathematical foundations of backpropagation.

### Exercises
- Calculate derivatives manually.
- Implement numerical differentiation.
- Compare numerical and analytical derivatives.
- Visualize gradients of two-variable functions.

## Module 6: Probability and statistics

**Duration:** 2 weeks

### Lessons
- Probability fundamentals
- Random variables
- Expected value
- Variance and standard deviation
- Probability distributions
- Gaussian distribution
- Conditional probability
- Bayes' theorem
- Entropy
- Information theory fundamentals

### Project
Create a Python probability simulator and visualize different probability distributions.

## Module 7: Classical machine learning

**Duration:** 2 weeks

### Learn
- Supervised and unsupervised learning
- Training and testing data
- Linear regression
- Logistic regression
- Classification
- Loss functions
- Overfitting and underfitting
- Regularization
- Cross-validation
- Evaluation metrics

### Projects
1. Linear regression from scratch.
2. Logistic regression from scratch.
3. Binary classification system.
4. Compare training and testing performance.

---

# Stage 3 — Neural Networks from Scratch (Months 5–6)

This is the central practical stage.

## Module 8: The artificial neuron

### Learn
- Biological inspiration
- Artificial neuron architecture
- Inputs
- Weights
- Biases
- Weighted sums
- Activation functions

The basic neuron is:

\[
z=\sum_{i=1}^{n}w_ix_i+b
\]

\[
a=f(z)
\]

Implement a neuron using only basic Python.

## Module 9: Activation functions

Learn and implement:

| Function | Purpose |
|---|---|
| Sigmoid | Binary probability outputs |
| Tanh | Outputs between -1 and 1 |
| ReLU | Common hidden-layer activation |
| Leaky ReLU | Helps address inactive ReLU units |
| Softmax | Multiclass probability distribution |

Plot every activation function and its derivative.

## Module 10: Forward propagation

### Learn
- Single-layer networks
- Multiple hidden layers
- Matrix-based computation
- Weight initialization
- Bias initialization
- Batch processing

Implement a network with configurable input, hidden, and output layers.

## Module 11: Loss functions

Learn:
- Mean squared error
- Mean absolute error
- Binary cross-entropy
- Categorical cross-entropy
- Negative log likelihood

Understand why different tasks require different loss functions.

## Module 12: Backpropagation

**Critical research foundation**

### Learn
1. Computational graphs
2. Derivatives of neural-network operations
3. Chain rule through multiple layers
4. Gradients of weights
5. Gradients of biases
6. Gradient accumulation
7. Parameter updates

The basic update rule is:

\[
W_{\text{new}}=W_{\text{old}}-\eta\nabla_W L
\]

Here, \(\eta\) is the learning rate.

Implement backpropagation manually without automatic differentiation.

## Module 13: Optimization

Learn:
- Batch gradient descent
- Stochastic gradient descent
- Mini-batch gradient descent
- Momentum
- RMSProp
- Adam
- Learning-rate scheduling

### Stage 3 major projects
1. Single-neuron implementation.
2. Perceptron classifier.
3. XOR neural network.
4. Multilayer perceptron.
5. MNIST digit classifier.
6. Neural-network library with your own forward and backward functions.

---

# Stage 4 — Deep Learning Architectures (Months 7–8)

Move beyond basic neural networks and understand architectures used in modern AI.

## Module 14: Deep neural networks

Learn:
- Deep versus shallow networks
- Vanishing gradients
- Exploding gradients
- Weight initialization (Xavier and He)
- Batch normalization
- Layer normalization
- Dropout
- Residual connections
- Skip connections

**Project:** Build a deep neural network and compare its training behavior with a shallow network.

## Module 15: Convolutional Neural Networks (CNNs)

### Learn
1. Image representation
2. Convolution operations
3. Filters and kernels
4. Feature maps
5. Padding and stride
6. Pooling
7. Flattening
8. CNN architecture
9. CNN backpropagation

### Projects
- Build convolution operations without deep-learning libraries.
- Train a CNN for handwritten digit recognition.
- Build an image classifier for multiple categories.

## Module 16: Recurrent Neural Networks

### Learn
- Sequential data
- Recurrent connections
- Hidden states
- Backpropagation through time
- Vanishing gradients in RNNs
- LSTM
- GRU

### Projects
- Predict the next number in a sequence.
- Build a basic text predictor.
- Compare RNN, LSTM, and GRU.

## Module 17: Attention and Transformers

### Learn
1. Attention mechanisms
2. Query, Key, and Value
3. Scaled dot-product attention
4. Self-attention
5. Multi-head attention
6. Positional encoding
7. Feed-forward networks
8. Residual connections
9. Layer normalization
10. Transformer architecture

An important equation is:

\[
Attention(Q,K,V)=
softmax\left(\frac{QK^T}{\sqrt{d_k}}\right)V
\]

### Projects
- Implement self-attention using NumPy.
- Build multi-head attention.
- Implement a small Transformer.
- Train a miniature language model on a small text dataset.

---

# Stage 5 — Advanced Deep Learning and Research Mathematics (Months 9–10)

This stage prepares you to understand research papers rather than simply use existing architectures.

## Module 18: Advanced mathematics

| Topic | Why it matters |
|---|---|
| Multivariable calculus | Deriving gradients |
| Matrix calculus | Understanding neural-network derivatives |
| Advanced linear algebra | Understanding transformations |
| Probability theory | Modeling uncertainty |
| Information theory | Understanding entropy and information |
| Numerical analysis | Understanding computational errors |
| Optimization theory | Understanding training algorithms |

### Additional subjects
- Jacobian matrices
- Hessian matrices
- Taylor series
- Convex and non-convex optimization
- Numerical stability
- Eigenvalue decomposition
- Singular value decomposition (SVD)

## Module 19: Advanced optimization

Learn:
- AdamW
- Learning-rate warmup
- Cosine learning-rate scheduling
- Gradient clipping
- Second-order optimization
- Adaptive optimization
- Weight decay
- Sharpness and generalization
- Loss landscape analysis

**Project:** Compare multiple optimizers on the same neural network and dataset. Analyze convergence speed, final loss, and generalization.

## Module 20: Generative models

Learn:
- Autoencoders
- Variational autoencoders (VAE)
- Generative adversarial networks (GANs)
- Diffusion models
- Latent spaces
- Generative modeling
- Sampling methods

### Projects
- Build an autoencoder.
- Implement a basic VAE.
- Build a small GAN.
- Experiment with a simplified diffusion process.

## Module 21: Large Language Models

Learn:
1. Tokenization
2. Embeddings
3. Vocabulary
4. Next-token prediction
5. Causal attention
6. Decoder-only Transformers
7. Pretraining
8. Fine-tuning
9. Instruction tuning
10. Evaluation and inference

**Project:** Build a small GPT-style language model from scratch, train it on a small text corpus, and examine its generated text.

---

# Stage 6 — Research and Independent Work (Months 11–12)

The goal is to move from following tutorials to asking and answering scientific questions.

## Module 22: Research methodology

Learn:
- How to read research papers
- How to identify a research problem
- Literature reviews
- Research hypotheses
- Experimental design
- Baseline models
- Ablation studies
- Reproducibility
- Statistical significance
- Writing research reports

## Module 23: Important research papers

Read these approximately in this order:

### 1. Learning representations by back-propagating errors (1986)
Understand how backpropagation became foundational to neural-network training.

https://www.nature.com/articles/323533a0

### 2. ImageNet Classification with Deep Convolutional Neural Networks (2012)
Understand the impact of deep CNNs and GPU training.

https://arxiv.org/abs/1207.0580

### 3. Attention Is All You Need (2017)
Understand the Transformer architecture.

https://arxiv.org/abs/1706.03762

### 4. BERT: Pre-training of Deep Bidirectional Transformers (2018)
Understand bidirectional language representation learning.

https://arxiv.org/abs/1810.04805

### 5. Language Models are Few-Shot Learners (2020)
Understand scaling and few-shot learning in large language models.

https://arxiv.org/abs/2005.14165

## Module 24: Conduct your first research experiment

Possible research questions:
- Does a different weight initialization improve training?
- How does network depth affect generalization?
- How does learning rate affect convergence?
- Does a particular activation function improve performance?
- How does attention behave when sequence length increases?

### Research workflow

1. Identify a research question.
2. Read related research papers.
3. Form a hypothesis.
4. Design a controlled experiment.
5. Implement the model.
6. Train and collect results.
7. Analyze and visualize results.
8. Write findings and limitations.

**Final project:** Produce a reproducible research report containing your hypothesis, mathematical explanation, implementation, experiments, results, and conclusions.

---

# 3. Development environment

You do not need an expensive computer or GPU to begin.

Install these tools:

| Tool | Purpose | Website |
|---|---|---|
| Visual Studio Code | Code editor | https://code.visualstudio.com/ |
| Python | Programming language | https://www.python.org/downloads/ |
| Jupyter Notebook | Interactive mathematical experiments | https://jupyter.org/ |
| Google Colab | Cloud notebooks and optional GPU access | https://colab.research.google.com/ |
| GitHub | Store code and research experiments | https://github.com/ |

**Important rule for your first six months:** Do not use PyTorch or TensorFlow to implement the core mathematical operations. Use Python and NumPy. Later, learn PyTorch to compare your implementation against a mature framework.

---

# 4. Books and learning resources

These resources should accompany the lessons, not replace practical implementation.

| Subject | Resource |
|---|---|
| Python | [Official Python Tutorial](https://docs.python.org/3/tutorial/) |
| Mathematics | [Khan Academy](https://www.khanacademy.org/math) |
| Linear algebra | [3Blue1Brown — Linear Algebra](https://www.3blue1brown.com/topics/linear-algebra) |
| Calculus | [Khan Academy — Calculus](https://www.khanacademy.org/math/calculus-1) |
| Machine learning | [Machine Learning Specialization](https://www.coursera.org/specializations/machine-learning-introduction) |
| Deep learning | [Deep Learning Specialization](https://www.deeplearning.ai/courses/deep-learning-specialization/) |
| Neural networks | [Neural Networks and Deep Learning](http://neuralnetworksanddeeplearning.com/) |
| Research papers | [arXiv](https://arxiv.org/) |

A particularly useful book later in your journey is *Deep Learning* by Ian Goodfellow, Yoshua Bengio, and Aaron Courville.

[Read Deep Learning online](https://www.deeplearningbook.org/)

---

# 5. Daily study routine

Recommended study time: approximately 2.5 hours per day, six days per week.

| Activity | Time |
|---|---:|
| Mathematics | 40 minutes |
| Python / programming | 40 minutes |
| Neural-network theory | 35 minutes |
| Practical exercises | 35 minutes |
| **Total** | **150 minutes** |

### Weekly structure
- Monday–Thursday: New lessons and exercises.
- Friday: Revision and problem solving.
- Saturday: Project implementation.
- Sunday: Rest or optional reading.

---

# 6. Progress milestones

Do not move to the next stage simply because you have watched all the lessons.

| Stage | Required achievement |
|---|---|
| 1 | Write Python programs independently |
| 2 | Understand matrices, derivatives, and probability |
| 3 | Implement backpropagation without automatic differentiation |
| 4 | Build CNN, RNN, and Transformer components |
| 5 | Explain advanced optimization mathematically |
| 6 | Reproduce a research experiment and write a report |

Aim to spend approximately 60% of your learning time solving problems and implementing code, rather than watching videos.

---

# 7. First seven days

## Week 1 — Python and mathematical thinking

| Day | Task |
|---|---|
| Day 1 | Install Python and VS Code. Write your first Python program. |
| Day 2 | Learn variables, numbers, strings, and basic arithmetic. |
| Day 3 | Learn conditions and comparison operators. |
| Day 4 | Learn loops and solve 10 programming problems. |
| Day 5 | Learn functions and write a mathematical calculator. |
| Day 6 | Learn algebraic expressions, variables, and simple equations. |
| Day 7 | Build a calculator and complete a Python fundamentals assessment. |

---

# 8. Your ultimate learning objectives

By the end of this program, the goal is for you to be able to:

1. Derive the mathematics behind neural networks.
2. Implement neural networks without machine-learning frameworks.
3. Understand backpropagation mathematically.
4. Design and experiment with new architectures.
5. Understand Transformers and language models.
6. Read and critically evaluate research papers.
7. Reproduce published experiments.
8. Develop and investigate your own research hypotheses.

## Final recommendation

Treat this as a university-style self-study program. Work through it one lesson at a time, with explanations, mathematical derivations, coding exercises, homework, and assessments.

Your first milestone is simple: **learn Python well enough to express mathematical ideas as working programs.** Everything else will build on that foundation.
