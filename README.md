# Simple RNN Implementation

This project provides a straightforward implementation of a Recurrent Neural Network (RNN) from scratch. The implementation is designed to demonstrate the fundamental concepts of RNNs, including the forward pass, backward pass, and parameter updates, making it a great starting point for understanding sequence modeling.

---

## Features

- **Custom RNN Implementation**: Builds the RNN from the ground up without relying on external deep learning libraries like TensorFlow or PyTorch.
- **Forward Pass**: Processes sequential data by iteratively updating hidden states and producing outputs.
- **Backward Pass**: Implements Backpropagation Through Time (BPTT) to compute gradients and adjust parameters.
- **Parameter Initialization**: Weights and biases are initialized and scaled to work well with the $\tanh$ activation function.
- **Training Loop**: Includes a simple loop for iteratively training the RNN using gradient descent.

---

## How It Works

### 1. Forward Pass
The forward pass processes the input sequence step by step:
- The hidden state is updated using input weights, hidden-to-hidden weights, and biases.
- Outputs are computed using the updated hidden states and output weights.

### 2. Backward Pass
The backward pass uses Backpropagation Through Time (BPTT) to:
- Compute gradients for parameters that affect both the current and future outputs.
- Accumulate these gradients across all time steps.
- Update weights and biases using gradient descent.

### 3. Training
The RNN is trained iteratively over multiple epochs, minimizing the loss function and adjusting parameters to improve performance.
