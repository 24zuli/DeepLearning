-> What is Deep Learning?
Deep learning is a subset of machine learning that utilizes multilayered neural networks, known as deep neural networks, to mimic the decision-making capabilities of the human brain. This approach enables computers to process complex data patterns and perform tasks such as classification, regression, and representation learning. Deep learning models are particularly effective with high-dimensional data, allowing them to identify intricate relationships within large datasets.

-> Types of Deep Learning Models:

- Feedforward Neural Networks (FNN): Also known as Multi-Layer Perceptrons (MLP), these are the simplest form of neural networks where information flows in one direction—from input to output—without feedback loops. They are commonly used for tasks like image classification and regression problems25.

- Convolutional Neural Networks (CNN): Designed for processing structured grid data such as images, CNNs automatically learn spatial hierarchies of features through convolutional layers. They excel in image recognition and computer vision tasks14.
- Recurrent Neural Networks (RNN): These networks are ideal for sequential data, such as time series or natural language processing. RNNs maintain a memory of previous inputs through feedback loops, making them suitable for tasks like speech recognition24.
- Long Short-Term Memory Networks (LSTM): A specialized type of RNN designed to remember long-term dependencies, LSTMs are effective in applications where context from earlier inputs is crucial, such as language modeling and translation35.
- Generative Adversarial Networks (GANs): Comprising two neural networks—a generator and a discriminator—GANs are used for generating new data samples that resemble a given dataset. They are widely applied in image synthesis and style transfer16.
- Transformers: These models leverage self-attention mechanisms to process data sequences in parallel, making them highly efficient for tasks like translation and text generation. Transformers have become foundational in natural language processing34.

-> Key Concepts in Deep Learning:

1) High-Dimensional Data:
-> Deep learning algorithms excel at handling high-dimensional data, allowing them to uncover patterns that simpler models might miss.

2) Training Process:
- Epochs: The number of complete passes through the training dataset.
- Forward Pass: The process where input data is fed through the network to produce an output.
- Backpropagation: A method used to update weights and biases by calculating gradients of the loss function with respect to each weight by the chain rule.

3) Loss Function Calculation:
->  The loss function quantifies how well the model's predictions match the actual outcomes. Common loss functions include:
  - Sparse Categorical Crossentropy: Used for multiclass classification problems.
  - Binary Crossentropy: Used for binary classification tasks.

4) Weights and Biases:
->  Initially, weights and biases are randomly initialized. As training progresses through multiple iterations (epochs), adjustments based on backpropagation improve model performance.

5) Tensors:
->  Tensors are multi-dimensional arrays that serve as the fundamental data structure in deep learning frameworks like TensorFlow. They can represent various types of data:

- Rank 0: Scalar
- Rank 1: Vector
- Rank 2: Matrix
- Higher ranks can represent more complex structures like batches of images or sequences.

6) Batch Processing:
->  Data is often processed in batches to optimize training efficiency:
- Batch Size: The number of samples processed before the model's internal parameters are updated.
For example, an image dataset might be represented with dimensions [128, 28, 28, 3], indicating a batch of 128 images with dimensions 28x28 pixels and 3 color channels (RGB).

7) Optimizers:
->  Optimizers adjust the weights during training to minimize the loss function. Common optimizers include:
-  Stochastic Gradient Descent (SGD)
-  Adam
-  RMSprop

8) Callbacks:
- Callbacks allow users to monitor training progress and implement custom actions based on model performance metrics, such as stopping training if accuracy does not exceed a certain threshold.
