<div align="center">

<img src="assets/banner.svg" alt="Synapse banner" width="100%" />

# Synapse

### Deep learning from scratch — no frameworks, no magic, just code, math, and intuition.

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](LICENSE.md)
[![Made with NumPy](https://img.shields.io/badge/built%20with-NumPy%20%2B%20Matplotlib-013243?logo=numpy&logoColor=white)](https://numpy.org)
[![Status](https://img.shields.io/badge/status-active%20learning%20journey-brightgreen)]()
[![PRs Welcome](https://img.shields.io/badge/discussions-welcome-blueviolet)](CONTRIBUTING.md)

</div>

## Why this repo exists

If you've ever called `model.fit()` and felt like you got the right answer for the wrong reason, this repo is for you.

Synapse is a from-scratch walk through deep learning. Build the simplest possible version of an idea first, watch it work (or fail), understand *why*, and only then reach for the abstraction that hides the details. Every algorithm here is implemented in plain Python with NumPy and Matplotlib before any framework enters the picture.

We start with a neuron learning to add two numbers, and end somewhere unexpected: looking at DNA and proteins through the same mathematical lens we used for images and text.

## How to read this repo

**Predict before you run.** Before executing a cell, guess what the output will be. Being wrong is where the learning happens.

**Break things on purpose.** Change a learning rate by 10x. Remove the activation function. Delete a layer. Watch what breaks and ask why.

**Inspect everything.** Print the weights. Plot the gradients. Watch the loss curve move (or refuse to). If a number flows through the network, you should be able to see it.

## The roadmap

### 01 — Numbers
*Where it all begins: a computer learning to add.*

The smallest possible neural network — one that learns `2 + 3 = 5` — written in about 100 lines. Every line is there for a reason: neurons, layers, the forward pass, ReLU, mean squared error, backpropagation, and gradient descent.

| Notebook | Focus |
|---|---|
| `adding_two_numbers.ipynb` | A full neural network from scratch: forward pass, loss, backprop, gradient descent |

### 02 — Images
*Numbers in a grid are still just numbers.*

Building a feedforward network for MNIST, then asking why that's not enough — motivating convolutions, pooling, batch normalization, and dropout from first principles.

### 03 — Text
*Sequences, attention, and the hardest problems so far.*

Tokenization, embeddings, recurrence, and the attention mechanism behind transformers. Ends with a miniature GPT.

### 04 — Biological
*Where the lines between code and life blur.*

Taking the sequence models from section 03 and pointing them at DNA, looking at protein structures, and closing the loop back to the neuron.

### 05 — Frameworks
*Now that you know what's happening inside...*

Every problem from sections 01–04 gets reimplemented in PyTorch and TensorFlow/Keras.

## Getting started

```bash
git clone https://github.com/MubiruEltonFelix1/synapse.git
cd synapse

python -m venv venv
source venv/bin/activate   # venv\Scripts\activate on Windows

pip install numpy matplotlib jupyter
jupyter notebook
```

No GPU required. Everything runs comfortably on a laptop CPU.

## Why "Synapse"

A synapse is the small gap between neurons where a signal crosses over and learning happens. It's the biological connection point this journey eventually arrives at, it's where information gets transformed and passed forward, and it's small and fundamental — the whole spirit of building from the smallest pieces.

## Inspirations

**Buri Gerhom**, lecturer at Mbarara University of Science and Technology, who taught the math underneath all of this.

**Andrej Karpathy**, whose *micrograd* and *Neural Networks: Zero to Hero* series shaped the "build it yourself" philosophy of this repo.

**3Blue1Brown**, whose neural network series remains the gold standard for visual intuition.

<div align="center">

*"What I cannot create, I do not understand." — Richard Feynman*

See [CONTRIBUTING.md](CONTRIBUTING.md) for how to get involved, and [LICENSE.md](LICENSE.md) for usage terms.

</div>
