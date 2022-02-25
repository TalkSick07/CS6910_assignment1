# CS6910_assignment1
This project is about building a feed forward neural network to be used to classify the dataset of the FASHION_MNIST dataset.
The dataset has 70000 examples in total. Each example belongs to one 10 classes - from 0 to 9.
For training, validation and testing 54000, 6000 and 10000 examples are used respectively.

The shape of each image is 28 x 28, it was flattened to the shape of 784 x 1. The class of each image is given as a number from 0 to 9, which has been hot-encoded by a defining a function called to_vector().
The activation functions used in the project are sigmoid, relu and tanh. For the output layer, softmax function is used to represent the probabilites of an image as belonging to all the classes. The class with the highest probability is conisdered as the predicted class. All the above functions have been defined in the code alongwith the codes for their derivatives.

We have also defined a function called Loss_Func which can calculate loss by two methods - cross-entropy and squared error.

The initialization of weights and biases is done by two methods - random and xavier. For this task, a function called init_weights_biases function has been defined.

Functions to perfrom forward propagation and backpropagation have been defined as forw_prop() and back_prop() respectively.

The alogorithms used for optimization are stochastic gradient descent (defined as StochasticGD()), momentum based gradient descent(MomentumBasedGD()), nesterov accelerated gradient descent(NesterovAGD()), root mean squared propagation(RMSProp()), adam(Adam()) and nesterov adam(Nadam()).

Steps to train and test a model:
1. Decide the no. of hidden layers, no. of neurons in each layer, activation function, learning algorithm, learning rate, batch size and other parameters depending on the chosen algorithm.
2. Initialize weights and biases using the function init_weights_biases().
3. Call the function corresponding to the chosen algorithm on the training dataset.
4. Use the Output() function and accuracy_score() function to get training accuracy. 
5. Similarly, find validation accuracy. The model with best validation accuracy is chosen.
6. Test the chosen model on the testing dataset by using the same procedure.
7. The accuracy on the test dataset represents the final resulting accuracy.

