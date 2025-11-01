**Note:** This work is in DRAFT phase. Use at your own will and risk.

# Building Backpropagation and Neural Networks from Scratch

## What This Notebook Is About

This notebook has two main goals:

1. **Implement backpropagation from scratch:** Build an automatic differentiation system that computes gradients automatically—the core mechanism behind all modern deep learning frameworks.

2. **Implement a Multi-Layer Perceptron (MLP) from scratch:** Build the fundamental components of neural networks (neurons, layers, and complete networks) and understand how they connect together.

Together, these two systems form a complete deep learning framework. At the end, we'll verify everything works by training our MLP on a simple prediction task.

## What We'll Build

**Automatic Differentiation System:**
- `Scalar` class that tracks operations and stores gradients
- Forward pass: Record all operations in a computation graph
- Backward pass: Automatically compute gradients using the chain rule
- Support for basic operations (addition, multiplication) and activation functions (ReLU)

**Neural Network Components:**
- `Neuron`: Single computational unit with weights and bias
- `Layer`: Collection of neurons that process inputs in parallel
- `MLP`: Multi-layer network that stacks layers together
- Parameter management and gradient handling

**Integration:**
- Connect backpropagation with neural networks
- Implement training loops: forward → loss → backward → update
- Demonstrate the complete system on a working example

By the end, you'll understand exactly how automatic differentiation works and how to build neural networks from first principles.
