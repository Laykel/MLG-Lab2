# MLG - Lab 2 : Neural network basics

## Activation functions

Activation functions are essential to artificial neural networks. They are used to compute the output of artificial neurons and therefore, the output of the network. An activation function must be differentiable if a learning algorithm like backpropagation wants to be used to find the network parameters.

This notebook shows some examples of activation functions, and how their shape change with respect to the weight of the connections between neurons.

## Simple perceptron neuron

Perceptrons are the building blocks of the most common type of artificial neural network: the Multi-Layer Perceptron. In this notebook you will explore how the output of a perceptron changes with respect to its inputs for different activation functions and different weight connections.

## Multi-Layer Perceptron (MLP)

A Multi-Layer Perceptron (MLP) is a collection of perceptrons connected and organized in layers. The output of one layer of perceptrons is the input of the next layer. Information travels through the network from input to output nodes. There are special configurations in which the information goes back to previous layers thanks to recurrent connections. Recurrent connections are out of the scope of this laboratory. In this notebook you are going to test how the output of a MLP changes with respect to the changes in its weight connections for different activation functions.

## Delta rule

_Very interesting and great interactive experiment in this file._

The Delta Rule is a gradient descent approximator that can be used to find the weight values of a Perceptron. The Delta Rule minimizes an error function (tipically 𝐸=12(𝑦−𝑡)2) by adapting the weight connections in small steps. The step length is defined by the learning rate 𝛼. In this notebook you will explore the classification capabilities of a single Perceptron by using the delta rule. You will start by setting the connection weights by hand for a simple problem, and then you will apply the delta rule for the same problem, and others.

## Backpropagation

The backpropagation algorithm is useful to find the weights and biases of a Multi-Layer Perceptron (MLP). It employs the chain rule of the derivative to find the direction in which the weight values need to be modified in order to minimize the error at the output. The algorithm performs in two phases: information is first propagated forward to compute the output of the network for a given input, and the error of the network; then, the error signal is propagated backwards and the network parameters are modified accordingly.
