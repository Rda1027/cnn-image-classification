# cnn-image-classification

The project was required as part of the practical exam for the course of Image Processing and Computer Vision in the Master's degree of Artificial Intelligence.

## Project Description

The project is divided into two parts:
- evaluation of performances of different CNNs built from scratch;
- fine tuning a pre-trained Resnet18.

The aim for the first section is to evaluate the performances of different kinds of CNNs, starting from the lowest accurate to the best one.
Showing that by adding components we manage to build classifiers that reach an higher level of accuracy.

The second section of the exam intended to evaluate the performances we managed to reach by fine tuning a Resnet18 pre-trained network.

## Implementation Details

The structures of the networks for the first section can be listed as:
1. MoreFullyConnectedNet: standard CNN + higher number of FC Layers (as a classification head);
2. NetWithoutBatchNorm: standard CNN + lower number of FC layers + lack of BatchNorm, Dropout and Residual Block layers;
3. NetWithoutResidualBlock: standard CNN + lower number of FC layers + BatchNorm layers + lack of Dropout and Residual Block layers;
4. NetWithoutDropout: standard CNN + lower number of FC layers + BatchNorm, Residual Block layers + lack of Dropout;
5. GroceryConvNet: standard CNN + lower number of FC layers + BatchNorm, Residual Block and Dropout layers.

The second section consisted in a single implementation of the Resnet18 network.
In particular, the network performances were evaluated, first, following specific training of the classification head ("transfer learning"), then by fine-tuning it.

For more details and better appreciate the results, it is suggested to explore the notebook ```assignment_module_2.ipynb```.

## Collaborators

- [Claudia Maiolino](https://github.com/jeanclaude8)
- [Valerio Costa](https://github.com/Rda1027)
