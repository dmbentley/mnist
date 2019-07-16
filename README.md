# Studying the MNIST dataset

Shown below is a representative 28 x 28 image of one of the handwritten digits. 

![](./images/digit.png)

## The First Model: Fully Connected

The first model is a fully connected neural network that achieves an accuracy of 96% with the following architecture:

* An initial *flat* layer of 784 neurons corresponding to each of the pixels in the 28x28 image.
* 5 hidden layers of 30 fully connected neurons each. These neurons will have a ReLU activation.
* A final layer of 10 neurons corresponding to the 10 digits. The neurons in this final layer will have a softmax activation. 

In addition:

The model will use:
* The adam optimizer
* Categorical cross entropy as a loss function to guide training
* Accuracy as a metric
* Be trained over 20 epochs

The model can be constucted and trained using Keras. Shown below are the accuracy and loss for both the training
and validation datasets.

![](./images/fully-connected-accuracy-loss.png)

As can be seen, the network begins to overfit to the training data around the 6th epoch. 

The model that is constucted has predicitive capabilities. Shown below are sample predictions that the network is able to
make. 

![](./images/grid-predictions.png)
