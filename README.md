# Activation Function Comparison in Neural Networks

This project compares the effects of three different activation functions — **ReLU**, **Sigmoid**, and **Tanh** — on the training performance of a simple neural network using the MNIST dataset.

## Objective

The goal of this experiment is to observe how the choice of activation function influences model accuracy, loss, and learning speed in a feedforward neural network trained for digit classification.

## Model Overview

- **Architecture**: MLP with two hidden layers (128 and 64 neurons)
- **Activation Functions Tested**: ReLU, Sigmoid, Tanh
- **Output Layer**: Softmax (10 classes for digits 0–9)

## Dataset

- **MNIST**: 70,000 grayscale images of handwritten digits (28x28 pixels)
- **Split**:
  - 60,000 for training/validation (80/20 split via `train_test_split`)
  - 10,000 for final testing

## Training Configuration

- Optimizer: Adam  
- Loss Function: Categorical Crossentropy  
- Batch Size: 128  
- Epochs: 10  
- Frameworks Used: TensorFlow/Keras, NumPy, scikit-learn, Matplotlib

## Results

- **ReLU** showed the best overall performance, with faster convergence and higher accuracy.
- **Tanh** performed reasonably well but slightly slower than ReLU.
- **Sigmoid** had the weakest performance due to vanishing gradient issues.

Visualizations include:
- Accuracy and loss curves
- Confusion matrices
- Graphs of the activation functions



