## Course Completed
- **[Building Deep Learning Models with TensorFlow](https://www.coursera.org/learn/building-deep-learning-models-with-tensorflow)**

## Important Notes to Remember

### Recurrent Neural Networks (RNNs):
- **RNN**: Suitable for sequential data like text and speech. Commonly used for applications such as language translation, voice recognition, and next-word prediction in text inputs.


### Restricted Boltzmann Machine (RBM):
- **Feature Learning**: Useful for dimensionality reduction, pattern recognition, and handling missing values.
- **Applications**: Widely used in recommender systems, specifically collaborative filtering.
- **Contrastive Divergence**: A learning algorithm used to train RBMs that approximates the gradient of the log-likelihood function.


### Deep Belief Networks (DBN):
- **Stack of RBMs**: A DBN is composed of multiple layers of RBMs where each layer learns to represent the data at a higher and more abstract level.
- **Removal of Backpropagation**: Traditionally, DBNs minimize the reliance on backpropagation by pre-training layers using an unsupervised approach.
- **Generative Models**: DBNs can be used to generate new data points by sampling from the learned distribution.

### Autoencoders:
- **Dimensionality Reduction**: Autoencoders are neural networks trained to attempt to copy their input to their output internally compressing the data in the process.
- **Feature Extraction**: They can learn codings that are useful for tasks such as anomaly detection or image reconstruction.
- **Variational Autoencoders (VAEs)**: A type of autoencoder that learns a probabilistic model of the data, allowing for the generation of new data points.

### Long Short-Term Memory (LSTM):
- **Language Modeling**: LSTMs are highly effective for tasks involving sequences, such as language modeling, due to their ability to capture long-term dependencies.
- **Vector Space Modeling**: Techniques like Word2Vec or GloVe represent words in a continuous vector space where similar words are mapped to nearby points.
- **Write, Read, and Forget Gates**: LSTMs use these gates to control the flow of information in and out of the cell.

### Others:
- **Eager Execution**: TensorFlow 2 default mode where operations are executed as they are defined. Useful for debugging and prototyping.
- **Curse of Dimensionality**: Refers to various phenomena that arise when analyzing and organizing data in high-dimensional spaces that do not occur in low-dimensional settings.
- **Principal Component Analysis (PCA)**: A statistical procedure that uses an orthogonal transformation to convert a set of observations of possibly correlated variables into a set of values of linearly uncorrelated variables called principal components.


**Tags**: TensorFlow, RNN, LSTM, RBM, Autoencoders, AI, Machine Learning, Deep Learning
