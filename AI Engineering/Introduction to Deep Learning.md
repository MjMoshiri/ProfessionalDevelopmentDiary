## Courses Completed
- **[Introduction to Deep Learning with Keras](https://www.coursera.org/learn/introduction-to-deep-learning-with-keras)** 

## Important Notes to Remember

### Gradient Problems:
- **Vanishing Gradient**: Occurs when gradients are too small, severely slowing down the training of deep neural networks. This can lead to the network failing to converge to a good solution.
- **Exploding Gradient**: Occurs when gradients are too large, causing the weights to update significantly and leading to instability in the training process.

### Activation Functions:
- **ReLU (Rectified Linear Unit)**: Commonly used activation function that helps mitigate the vanishing gradient problem by allowing models to learn faster and perform better.
- **Sigmoid**: Activation function that squashes the output between 0 and 1, useful in binary classification problems, but can suffer from the vanishing gradient problem.
- **Tanh (Hyperbolic Tangent)**: Activation function that squashes the output between -1 and 1, useful in binary classification problems, but can suffer from the vanishing gradient problem.
- **Softmax**: Activation function that squashes the output between 0 and 1, useful in multi-class classification problems.
### Convolutional Neural Networks (CNN):
- **Convolutional Layer (Filters)**: Applies a set of learnable filters to the input image to create feature maps, capturing important features such as edges, shapes, etc.
- **Pooling Layer**: Reduces the spatial size of the feature maps, decreasing the number of parameters and computation in the network, and helps in making the detection of features invariant to scale and orientation.

### Recurrent Neural Networks (RNN):
- **Long Short-Term Memory (LSTM)**: A type of RNN capable of learning order dependence in sequence prediction problems. It addresses the issue of long-term dependencies where standard RNNs fail.
- **Restricted Boltzmann Machines (RBMs)**: A stochastic neural network that can learn a probability distribution over its set of inputs, useful in dimensionality reduction, classification, regression, collaborative filtering, feature learning, and topic modeling.

### Other Key Concepts:
- **Autoencoders**: A type of neural network used for unsupervised learning that learns how to efficiently encode and compress data, useful in dimensionality reduction, data denoising, and anomaly detection.
- **Batching**: The process of dividing the training data into smaller batches to speed up the training process and reduce memory requirements.
