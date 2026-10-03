# Neural Network Linear Regression from Scratch

## 📌 Overview

This project demonstrates the implementation of a simple neural network from scratch using Python and NumPy.

The model is designed to learn a simple linear relationship between two input features and an output:

y = 3x1 + 4x2

For the given input values:

- x1 = 3
- x2 = 2

the actual output is:

y = (3 × 3) + (4 × 2) = 17

The model starts with randomly initialized weights and learns to produce a prediction close to the actual value by using feed-forward computation, error calculation, backpropagation, and gradient descent.

---

## 🎯 Objective

The main objective of this project is to understand how a basic neural network learns from data.

The project demonstrates:

- Random weight initialization
- Feed-forward computation
- Prediction calculation
- Squared error calculation
- Backpropagation
- Gradient calculation
- Weight updating
- Gradient descent
- Training over multiple epochs
- Visualization of training progress

---

## 🧠 Problem Statement

The neural network needs to learn the following relationship:

y = 3x1 + 4x2

Given:

x1 = 3

x2 = 2

The expected output is:

y = 17

Initially, the model does not know the correct weights.

It starts with random weights:

- w1
- w2

The model then adjusts these weights during training so that the predicted output approaches the actual output.

---

## 🔄 Methodology

The model follows these steps:

1. Initialize random weights between 1 and 10.
2. Define the input features and actual output.
3. Perform feed-forward computation.
4. Calculate the predicted output.
5. Calculate the squared error.
6. Calculate gradients using backpropagation.
7. Update the weights using gradient descent.
8. Repeat the process for multiple epochs.
9. Store the error and prediction values.
10. Visualize the learning process using graphs.

---

## 📐 Mathematical Formulas

### Prediction

The predicted output is calculated as:

y_pred = x1 × w1 + x2 × w2

---

### Error Calculation

The squared error is:

Error = (y_actual - y_pred)²

Squaring the error makes the error non-negative and provides a value that can be minimized during training.

---

### Gradient of w1

The gradient with respect to w1 is:

gradient_w1 = -2 × x1 × (y_actual - y_pred)

---

### Gradient of w2

The gradient with respect to w2 is:

gradient_w2 = -2 × x2 × (y_actual - y_pred)

---

### Weight Update

The weights are updated using gradient descent:

w1 = w1 - learning_rate × gradient_w1

w2 = w2 - learning_rate × gradient_w2

---

## 📊 Sample Data

| Parameter | Value |
|-----------|------:|
| x1 | 3 |
| x2 | 2 |
| Actual y | 17 |

The actual output is calculated as:

3 × 3 + 4 × 2 = 17

---

## ⚙️ Technologies Used

- Python
- NumPy
- Matplotlib
- Jupyter Notebook

---

## 📚 Concepts Used

### 1. Neural Network

A neural network is a machine learning model that learns relationships between inputs and outputs by adjusting weights.

### 2. Feed Forward

Feed forward is the process of passing input values through the model to calculate a predicted output.

### 3. Error

Error measures the difference between the actual output and predicted output.

### 4. Backpropagation

Backpropagation calculates the gradients of the error with respect to the weights.

### 5. Gradient Descent

Gradient descent updates the weights in a direction that reduces the error.

### 6. Learning Rate

The learning rate controls how much the weights change during each update.

### 7. Epoch

An epoch represents one complete training iteration.

---

## 🔧 Activation Functions

The project also defines three commonly used neural-network activation functions:

### Sigmoid

Sigmoid produces values between 0 and 1.

### Tanh

Tanh produces values between -1 and 1.

### ReLU

ReLU returns the input value when it is positive and returns 0 for negative values.

These functions are included to demonstrate common neural-network activation functions. The simple linear regression calculation in this project uses the direct weighted-sum equation for prediction.

---

## 📈 Results

During training, the model updates its weights to reduce the prediction error.

The expected behavior is:

- Error decreases toward zero.
- Predicted Y approaches 17.
- Learned w1 approaches 3.
- Learned w2 approaches 4.

The exact values can vary depending on the initial random weights and learning rate.

---

## 📊 Visualizations

### Error Progression

The error is plotted against the number of epochs.

The graph demonstrates how the training error decreases as the model learns.

### Predicted Y Progression

The predicted output is plotted against the epochs.

The prediction gradually approaches the actual value:

17

