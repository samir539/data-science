# Back Propagation

Back Propagation is a fundamental concept in the field of artificial neural networks and is an essential part of training multilayer perceptrons (MLPs). It is an optimization algorithm used to adjust the weights and biases of the neural network during the training process.

The main steps of the Back Propagation algorithm are as follows:

1. Forward Pass: During the forward pass, the input data is propagated through the network, layer by layer, using the current weights and biases. The activations of each neuron are calculated, and the output is obtained.

2. Compute Loss: The difference between the predicted output and the actual target (loss function) is computed to quantify the model's performance.

3. Backward Pass: In the backward pass, the gradients of the loss with respect to the weights and biases are computed using the chain rule of calculus. This step involves calculating the partial derivatives of the loss function with respect to the model's parameters.

4. Update Weights and Biases: Using the computed gradients, the weights and biases of the neural network are updated to minimize the loss function. This update is done using optimization algorithms like stochastic gradient descent (SGD).

The Back Propagation algorithm allows the neural network to iteratively learn from the training data, adjusting its parameters to minimize the prediction error and improve its performance.

# MLPs and SGD

Multilayer Perceptrons (MLPs) are a type of artificial neural network consisting of multiple layers of interconnected neurons. They can be used for a wide range of machine learning tasks, including classification, regression, and pattern recognition.

SGD, short for Stochastic Gradient Descent, is a popular optimization algorithm used to train MLPs. It works by updating the model's parameters (weights and biases) in the direction of the negative gradient of the loss function for a randomly selected subset of training data (a mini-batch).

The main steps of the SGD algorithm are as follows:

1. Initialize Parameters: The weights and biases of the MLP are initialized with random values.

2. Forward Pass: During the forward pass, the input data is propagated through the network to calculate the model's predictions.

3. Compute Loss: The difference between the predicted output and the actual target (loss function) is computed to quantify the model's performance.

4. Backward Pass: The gradients of the loss with respect to the model's parameters are computed using the Back Propagation algorithm.

5. Update Weights and Biases: Using the computed gradients, the weights and biases of the MLP are updated in the direction that reduces the loss function.

6. Repeat Steps 2-5: The process is repeated for multiple iterations (epochs) or until convergence to find the optimal set of parameters.

MLPs trained using SGD have the ability to learn complex patterns and relationships from the data, making them a powerful tool in various machine learning applications.

