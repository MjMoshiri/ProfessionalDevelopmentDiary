## Course Completed
- **[Deep Neural Networks with PyTorch](https://www.coursera.org/learn/deep-neural-networks-with-pytorch)**

## Important Notes to Remember

### PyTorch Basics:

- **required_grad**: Used in PyTorch to indicate whether a tensor should be tracked for gradient calculations.
- **transform**: Techniques to modify raw data making it suitable for training neural networks, like normalization and augmentation.
- **lazy**: In PyTorch, refers to modules and operations that delay computation until needed, improving efficiency.
- **PyTorch Cuda**: Utilizes Nvidia GPUs for tensor calculations, significantly speeding up the training process.
- **DataLoader**: A PyTorch class that provides an efficient way to load and iterate over data samples during training.


### Optimization Techniques:
- **Stochastic Gradient Descent (SGD)**: An optimization method that updates parameters in small batches, averaging over a subset of the total data.
- **Velocity**: In optimization algorithms like SGD with momentum, it helps to accelerate SGD in the relevant direction and dampens oscillations. Helps to converge faster, avoiding local minimum, and saddle points. 

### Loss Functions and Regularization Techniques:
- **Cross-Entropy Loss**: Measuring the performance of a classification model whose output is a probability.
- **DropOut**: A regularization technique to prevent overfitting by randomly setting a fraction of input units to zero at each update during training time.
- **Batch Normalization**: Technique to improve the training of deep neural networks by stabilizing learning processes and dramatically reducing the number of training epochs required.
  - **Benefits**: Reduces internal covariate shift, can remove the need for Dropout, allows for higher learning rates, and Biases are not necessary.

### Weight Initialization Techniques:

- **Xavier**: Keeps the scale of gradients roughly the same in all layers.
- **Kaiming He**: Random number with a Gaussian distribution, mean 0, and variance 2/n, where n is the number of input units in the weight tensor. Paritcularly useful for ReLU activation functions.


### Convolutional Neural Networks (CNNs):
- **Activation maps**: Intermediate outputs of a CNN that represent the presence of particular features in an image.
- **Stride**: The number of pixels by which the filter slides over the input image.
- **Padding**: Adding extra pixels around the input image.
- **Torch Vision**: A part of the PyTorch ecosystem that provides tools and datasets for computer vision tasks.
    - **ResNet18**: A model from the ResNet family with 18 layers, commonly used in many vision tasks due to its efficiency and accuracy.

**Tags**: PyTorch, Machine Learning, Neural Networks, Deep Learning, AI
