# Perceptron:-
   A perceptron is a type of artificial neuron that serves as the simplest form of a neural network, specifically designed for binary classification tasks. It operates as a single-layer classifier, meaning it consists of only one layer of output nodes directly connected to the input features. The perceptron model can be mathematically represented as follows:

1. Weighted Sum Calculation:
- The perceptron computes a weighted sum of its inputs:
  
  <img src = "https://github.com/user-attachments/assets/7528690a-260f-4693-82e6-57df43c1471a" width = "150"/>

  where:
  - z is the weighted sum,
  - w<sub>i</sub> are the weights corresponding to each input,
  - x<sub>i</sub> are the input features,
  - b is the bias term.

2. Activation Function:
- The output of the perceptron is determined by applying a step function (also known as a Heaviside step function) to the weighted sum:
  
  <img src = "https://github.com/user-attachments/assets/f0b32ff9-c4df-4b45-a343-cea150163d50" width = "150"/>

  This function outputs 1 if the weighted sum is greater than zero and 0 otherwise, effectively creating a linear decision boundary.

  
3. Logistic Function:
- The probability that an instance belongs to class 1 is given by:
  
  <img src = "https://github.com/user-attachments/assets/34e22efd-9b58-4177-a7b5-1cc71e131e45" width= "300">

4. Decision Boundary:
- A threshold (commonly set at 0.5) determines class membership:
  - If P(y=1∣x) > 0.5, classify as class 1.
  - Otherwise, classify as class 0.
 
# Multi layer Perceptron:

A Multi-Layer Perceptron (MLP) is a type of artificial neural network that consists of multiple layers of neurons. Unlike a single layer perceptron, which can only represent linear functions, an MLP can approximate complex non-linear functions due to its multiple layers and interconnected neurons. The flow of information in an MLP is termed feedforward, as data moves in one direction from input to output without any cycles or feedback loops.

-> Structure of MLPs: 
- Input Layer: This layer receives the input features.
- Hidden Layers: One or more layers where computations occur. Each neuron in these layers applies a weighted sum followed by a non-linear activation function.
- Output Layer: Produces the final output, which can be a single value (for regression) or probabilities for classification tasks.

-> Feedforward Process:

- Input Layer: Inputs x<sub>1</sub>,x<sub>2</sub>,…,x<sub>n</sub> are fed into the network.
- Hidden Layer(s): Each neuron computes a weighted sum of its inputs and applies an activation function.
- Output Layer: The final layer produces the output based on the computations from the hidden layers.

-> Calculations:

1. Hidden Layer Calculation:
   
   <img src = "https://github.com/user-attachments/assets/3f0d2531-796d-4f6b-a0e5-5d1c73e0da72" width = "200"/>

  where:
   - z<sub>h</sub> is the vector of hidden layer outputs,
   - W<sub>h</sub> is the weight matrix for the hidden layer,
   - b<sub>h</sub> is the bias vector for the hidden layer,
   - x is the input vector.

2. Activation Function for Hidden Layer:

   a<sub>h</sub> = f(z<sub>h</sub>)

   where:
   - f is a non-linear activation function (e.g., ReLU, sigmoid).

3. Output Layer Calculation:
   
   z<sub>o</sub> = W<sub>o</sub>a<sub>h</sub> + b<sub>o</sub>

   where:
   - z<sub>o</sub> is the output layer's weighted sum,
   - W<sub>o</sub> is the weight matrix for the output layer,
   - b<sub>o</sub> is the bias for the output layer.

4. Final Output Activation:
   
   y = g(z<sub>o</sub>)
   
   where:
   - g is typically a softmax or sigmoid function depending on whether it's a multi-class or binary classification task.


## Example:

$$f(x) = 2sin(x^2) + \sqrt{5x}$$

We can break this down into component functions and represent it using an MLP structure:

-> Functions Defined:
- $$f1 = add()$$: Adds two values.
- $$f2 = \sqrt()$$: Computes square root.
- $$f3 =\sqrt()$$: Computes square root (for another term).
- $$f4 = sin()$$: Computes sine.
- $$f5 = mul()$$:  Multiplies two values.

 <img src = "https://github.com/user-attachments/assets/f557f9b7-79c2-40c0-987c-412bb20b0c0a" width = "350" />

-> Explanation of Diagram: 
   - The input x flows into two branches:
      - The first branch computes $x^2$, which then goes to the sine function $f_4=sin()$. The result is multiplied by 2 using function $f_5=mul()$.
      - The second branch computes $5x$ which then goes to the square root function $f_2=\sqrt()$.
      - Both results are then combined using function 
$$f_1=add()$$ to produce the final output $$y=2sin(x^2)+\sqrt(5x)$$.


-> It prones to Overfitting and Underfitting but how?
- Overfitting:
  Overfitting occurs when an MLP learns the training data too well, including its noise and outliers, leading to poor generalization on unseen data. This happens due to several factors:
   - High Model Complexity
   - Insufficient Training Data
   - Long Training Periods
   - Noisy Data
   - Error = Bias<sup>2</sup> +Variance + Irreducible Error
 
- Underfitting:
  Underfitting occurs when an MLP is too simplistic to capture the underlying patterns in the data. This leads to poor performance on both training and unseen data.
   - Too Simple Model
   - Insufficient Features
   - Excessive Regularization
   - Low Variance
   - Error = Bias<sup>2</sup> + Variance + Irreducible Error
 
- Balancing Overfitting and Underfitting:
    - Regularization Techniques
    - Cross-Validation
    - Early Stopping
    - Data Augmentation
    - Feature Engineering

     






