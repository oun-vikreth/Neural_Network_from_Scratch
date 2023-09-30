# Neural_Network_from_Scratch
Try to build a neural network from scratch by only use some basic python's libraries such as Numpy,... etc. 

Certainly! Here's the documentation written in Markdown format:

```markdown
# Digit Recognition Neural Network

This project implements a neural network for digit recognition using the MNIST dataset. The neural network is trained using gradient descent and achieves high accuracy in classifying handwritten digits.

## Table of Contents

- [Installation](#installation)
- [Usage](#usage)
- [Dataset](#dataset)
- [Model Architecture](#model-architecture)
- [Training](#training)
- [Testing](#testing)
- [Results](#results)
- [Contributing](#contributing)
- [License](#license)

## Installation

To use this project, you need to have Python 3.x installed on your system. You also need to install the following dependencies:

- numpy
- pandas
- matplotlib

You can install these dependencies by running the following command:

```
pip install numpy pandas matplotlib
```

## Usage

To use the digit recognition neural network, follow these steps:

1. Clone the repository:

```
git clone https://github.com/your-username/digit-recognition.git
```

2. Change into the project directory:

```
cd digit-recognition
```

3. Run the `train.py` script to train the neural network:

```
python train.py
```

4. Run the `test.py` script to test the neural network on a specific image:

```
python test.py
```

## Dataset

The MNIST dataset consists of 60,000 training images and 10,000 test images of handwritten digits. Each image is a 28x28 grayscale image, representing a digit from 0 to 9.

## Model Architecture

The neural network architecture consists of the following layers:

- Input layer: 784 units (corresponding to the 28x28 pixel image)
- Hidden layer: 10 units
- Output layer: 10 units (corresponding to the 10 possible digit classes)

The activation function used in the hidden layer is the rectified linear unit (ReLU), and the output layer uses the softmax activation function.

## Training

The neural network is trained using gradient descent. The weights and biases are initialized randomly, and the network is trained for a specified number of iterations. The learning rate is set to 0.1. The training process involves forward propagation, backpropagation, and weight updates.

The backpropagation algorithm computes the gradients of the weights and biases using the following formulas:

- Gradient of the weights in the output layer:

```
dW2 = (1/m) * (A2 - Y) * A1.T
```

- Gradient of the biases in the output layer:

```
db2 = (1/m) * sum(A2 - Y)
```

- Gradient of the weights in the hidden layer:

```
dW1 = (1/m) * (W2.T * (A2 - Y)) * deriv_ReLU(Z1) * X.T
```

- Gradient of the biases in the hidden layer:

```
db1 = (1/m) * sum(W2.T * (A2 - Y)) * deriv_ReLU(Z1)
```

## Testing

After training, you can test the neural network on a specific image from the training set. The `test.py` script selects an image randomly and displays the image along with the predicted label. This can be useful to visually inspect the performance of the neural network.

## Results

The neural network achieves high accuracy in classifying handwritten digits. The accuracy is printed at every 50th iteration during training. The final accuracy on the test set can be used as a measure of the performance of the neural network.

## Contributing

Contributions to this project are welcome. If you find any issues or have suggestions for improvements, please open an issue or submit a pull request.

## License

This project is licensed under the [MIT License](LICENSE). You are free to use, modify, and distribute this code for personal or commercial purposes.
```

Save the above content in a file with the extension `.md`, such as `README.md`, to create a Markdown file for your project's documentation.
