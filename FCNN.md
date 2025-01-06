A Fully Connected Neural Network (FCNN) is a type of artificial neural network where each neuron in one layer is connected to every neuron in the next layer. This architecture allows the network to learn complex relationships in data through multiple layers of transformation.

- Input Layer: The layer that receives input data.
- Hidden Layers: Intermediate layers that transform inputs into outputs.
- Output Layer: The final layer that produces the output predictions.

-> Input and Output:
- Let $D = {x_i,y_i}$ represent a dataset where:
   - $x_i\epsilon R^n$ : Input Features(e.g., $x_1,x_2,x_3$ ).
   - $y_i\epsilon R$: Target Output.
     
-> Neuron Output:
- $o_{ij}$: Output from the i-th layer from the j-th neuron.

-> Representation: 

<img src = "https://github.com/user-attachments/assets/b5871741-38c8-4ea0-b48e-6d4d46cd09a8" width = "200"/>

- Here, 
  - $x_{ij}$ : i = point index and j = feature
  - $f_{ij}$ : i = layer number and j = function index
  - $w_{ij}$ : next layer index where i = from which point/neuron and j = to which point/neuron
               
-> Weights: 
- Weight Matrix W1: Connects the input layer to the first hidden layer.
- Weight Matrix W2: Connects the first hidden layer to the second hidden layer.
- Weight Matrix W3: Connects the second hidden layer to a third hidden layer (if applicable).
- Weight Matrix W4: Connects the third hidden layer to the output layer.

- The weight matrix $W_1$(Input to Hidden Layer 1):
     
     - An input layer with 3 features.
     - A first hidden layer with 4 neurons.
   
   <img src = "https://github.com/user-attachments/assets/fd3842da-5c53-4728-8762-efd756240b89" width = "200" />

- Weight Matrix $W_2$(Hidden Layer 1 to Hidden Layer 2):
  
    - A first hidden layer with 4 neurons.
    - A second hidden layer with 3 neurons.
  
  <img src = "https://github.com/user-attachments/assets/37e78616-6947-4782-837f-d0d93d81bc86" width = "200" />

- Weight Matrix $W_3$(Hidden Layer 2 to Hidden Layer 3):
  
   - A second hidden layer with 3 neurons.
   - A third hidden layer with 2 neurons.
 
     <img src = "https://github.com/user-attachments/assets/1e656e7b-22f4-445e-a752-8fee375b84ba" width = "200" />

- Weight Matrix $W_4$(Hidden Layer 3 to Output Layer):

   - A third hidden layer with 2 neurons.
   - An output layer with 1 neuron.

     <img src = "https://github.com/user-attachments/assets/3fcbc149-350b-4f72-a89c-36cc0a4d8c9f" width = "200" />

### Example:

<img src = "https://github.com/user-attachments/assets/5fd71c71-eca2-4ce3-8f1d-46e80409eeb4" width = "150"/> 

<img src = "https://github.com/user-attachments/assets/9ce68178-d213-4e14-a2fb-1c0fc3c16ef3" width = "150" /> 

<img src = "https://github.com/user-attachments/assets/9ab14624-2eda-49ce-956d-b51fc91f5a8d" width = "150" />

<img src = "https://github.com/user-attachments/assets/f189c39f-8304-48d0-8101-9fd88ba7b9e0" width = "150"/>








  
  

  
