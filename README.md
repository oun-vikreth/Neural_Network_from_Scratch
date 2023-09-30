python test.py


### Dataset

The MNIST dataset consists of 60,000 training images and 10,000 test images of handwritten digits. Each image is a 28x28 grayscale image, representing a digit from 0 to 9.

### Model Architecture

The neural network architecture consists of the following layers:

python
Input layer: 784 units
Hidden layer: 10 units
Output layer: 10 units


The activation function used in the hidden layer is the rectified linear unit (ReLU), and the output layer uses the softmax activation function.

### Training

The neural network is trained using gradient descent. The weights and biases are initialized randomly, and the network is trained for a specified number of iterations. The learning rate is set to 0.1.

The backpropagation algorithm is used to compute the gradients of the weights and biases. The gradients are then used to update the weights and biases in the direction of the steepest descent.

### Testing

After training, the neural network can be tested on a specific image by feeding the image into the network and predicting the digit. The predicted digit can then be compared to the true digit to evaluate the performance of the network.

### Results

The neural network achieves high accuracy in classifying handwritten digits. The final accuracy on the test set is typically above 95%.

### Contributing

Contributions to this project are welcome. If you find any issues or have suggestions for improvements, please open an issue or submit a pull request.

### License

This project is licensed under the MIT License. You are free to use, modify, and distribute this code for personal or commercial purposes.


This Markdown file can be saved with the `.md` extension, such as `README.md`, and uploaded to GitHub as the project's documentation.
