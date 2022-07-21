# Neural Network built from scratch
## Functioning of a Neural Network
### Weights and biases
For each of the inputs we provide to the Neural network, we associate some 'values' with each one of them. Now, these values determine how much importance has to be given to which attribute from the input, in order to predict more better results.  
Bias is used to just shift the activation function towards left or right, because it only adds or subtracts a constant value from the input, we will be giving into the activation function.
### Activation Function
In many cases if we want to normalise the output of our model, maybe for some scale purpose or for better observations, activations function come into play to normalise the output of any input in the range between 1 to -1 or 0 to 1.  
They also help us to introduce non-linearity in a model. Like not just having a step-function taking '0' and '1' but it can take other values as well, maybe 0.7 or 0.14.  
Sigmoid, ReLU and softmax are some common examples of activation functions, implemented in the NNs.  
Moreover, different types of activation functions are used in different layers specifically, in order to better optimise the output of the model.
### Gradient Descent
Gradient Descent is an optimization algorithm that is used to minimize a function by slowly moving in the direction of steepest descent, which is defined by the negative of the gradient.
So, it basically helps to minimize the objective convex function f(x) to its minimum using iterations.
We use this concept to reduce the cost/loss function and thus reaching to 'more' better values of weights and baises, for our model. Like in my model, I just randomly initialised the weights and biases, and after that, techniques like these are really helpful towards predicting their pretty good values.
### Learning Rate
In the gradient descent function it represents the size of each step down towards the bottom point.
But learning rate must be chosen wisely as well as if it is too small, then the model will take too much time to learn, but even if it is too large, the model will converge as our pointer will shoot and we’ll not be able to get to minima.
### Back propagation
When after implementing all the above components into our neural network, we try experimenting it on some test data, then we are likely to not get that accurate results or which are not satisfactory. In such cases, we try to back propagate to the previous layers of our model, and then update the weights and accordingly, and thus to the next previous layer and so on till we reach the input layer. Now, we are able to change the intermidatary outputs, just as we know as to how our results are not satisfactory and implement the changes accordingly.