Sure! Here's the updated version with the code and math formulas formatted in Markdown:

## Digit Recognition Neural Network

### Introduction

This project implements a neural network for digit recognition using the MNIST dataset. The neural network is trained using gradient descent and achieves high accuracy in classifying handwritten digits.

### Backpropagation Formulas

The following formulas are used to compute the gradients of the weights and biases in the backpropagation algorithm:

Gradient of the weights in the output layer:

```
dW2 = (1/m) * (A2 - Y) * A1.T
```

Gradient of the biases in the output layer:

```
db2 = (1/m) * sum(A2 - Y)
```

Gradient of the weights in the hidden layer:

```
dW1 = (1/m) * (W2.T * (A2 - Y)) * deriv_ReLU(Z1) * X.T
```

Gradient of the biases in the hidden layer:

```
db1 = (1/m) * sum(W2.T * (A2 - Y)) * deriv_ReLU(Z1)
```

where:

- `m` is the number of training examples
- `A2` is the output of the hidden layer
- `Y` is the ground truth labels
- `W2` is the weight matrix between the hidden layer and the output layer
- `db2` is the bias vector for the output layer
- `Z1` is the output of the hidden layer before the activation function
- `deriv_ReLU(Z1)` is the derivative of the ReLU activation function evaluated at `Z1`
- `W1` is the weight matrix between the input layer and the hidden layer
- `db1` is the bias vector for the hidden layer

### Usage

To use the backpropagation formulas, you would first need to calculate the output of the network for each training example. This can be done using the following steps:

1. Calculate the output of the hidden layer for each training example:

```
Z1 = W1 * X + b1
```

2. Apply the ReLU activation function to the output of the hidden layer:

```
A1 = relu(Z1)
```

3. Calculate the output of the output layer for each training example:

```
Z2 = W2 * A1 + b2
```

4. Apply the softmax activation function to the output of the output layer:

```
A2 = softmax(Z2)
```

Once the output of the network has been calculated for each training example, you can then use the backpropagation formulas to compute the gradients of the weights and biases.

The gradients can then be used to update the weights and biases of the network using the following steps:

1. Update the weights in the output layer:

```
W2 = W2 - learning_rate * dW2
```

2. Update the biases in the output layer:

```
b2 = b2 - learning_rate * db2
```

3. Update the weights in the hidden layer:

```
W1 = W1 - learning_rate * dW1
```

4. Update the biases in the hidden layer:

```
b1 = b1 - learning_rate * db1
```

By repeating these steps, the network will gradually learn to classify handwritten digits more accurately.

### Results

The neural network achieves high accuracy in classifying handwritten digits. The final accuracy on the test set is typically above 95%.

### Contributing

Contributions to this project are welcome. If you find any issues or have suggestions for improvements, please open an issue or submit a pull request.

### License

This project is licensed under the MIT License. You are free to use, modify, and distribute this code for personal or commercial purposes.
