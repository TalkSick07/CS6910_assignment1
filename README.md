# CS6910_assignment1
This project is about building a feed forward neural network to be used to classify the dataset of the FASHION_MNIST dataset.
The dataset has 70000 examples in total. Each example belongs to one 10 classes - from 0 to 9.
For training, validation and testing 54000, 6000 and 10000 examples are used respectively.

The activation functions used in the project are sigmoid, relu and tanh. For the output layer, softmax function is used to represent the probabilites of an image as belonging to all the classes. The class with the highest probability is conisdered as the predicted class. All the above functions have been defined in the code alongwith the codes for their derivatives.

We have also defined a function called Loss_Func which can calculate loss by two methods - cross-entropy and squared error.

The initialization of weights and biases is done by two methods - random and xavier. For this task, a function called init_weights_biases function has been defined.

Functions to perfrom forward propagation and backpropagation have been defined as forw_prop() and back_prop() respectively.

The alogorithms used for optimization are stochastic gradient descent (defined as StochasticGD()), momentum based gradient descent(MomentumBasedGD()), nesterov accelerated gradient descent(NesterovAGD()), root mean squared propagation(RMSProp()), adam(Adam()) and nesterov adam(Nadam()).



