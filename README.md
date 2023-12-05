# Custom Neural Network for MNIST Number Prediction

This repository, named Custom-N_N-MNIST, houses a custom neural network tailored for predicting numerical values from the MNIST dataset. For a detailed explanation and walkthrough, please refer to the [Evernote document](https://www.evernote.com/shard/s560/sh/df35c6e5-5e37-f971-e7ad-c4db04781d2f/Cdk1JcZ343w5S4fdcTYm7rBs9X91usVNe_wKpKCDuFV3O0oapFpozXSN2g) or access the PDF file located in the repository's root directory.

## Overview

The neural network begins with the preprocessing of image data, transforming it into a 28 x 28 format, resulting in an image output represented by 784 bits. The dataset is structured as a matrix of size 784 x n, where n corresponds to the number of images. The architecture of the neural network consists of an initial/input layer (a0) with 784 nodes, two hidden layers (z1 and z2) each containing 10 nodes, and a final output layer.

## Processing Steps

1. **Initial/Input Layer (a0):** Comprising 784 nodes, each node corresponds to a bit in the image representation.

2. **First Hidden Layer (z1):** This layer involves a weighted sum operation (z1 = w1 * a0 + b), where w1 represents the weights associated with each node, and b denotes the bias term.

3. **Second Hidden Layer (z2):** Similar to the first hidden layer, this step computes a weighted sum (z2 = w2 * a1 + b), where a1 is the output from the first hidden layer.

4. **Softmax Activation:** After processing through the hidden layers, the resulting values are passed through the softmax activation function. This converts the raw output into probability scores, indicating the likelihood of the input image representing a particular number.

## Accessing the Explanation

For a comprehensive explanation of the neural network's development and operation, please visit the [Evernote document](https://www.evernote.com/shard/s560/sh/df35c6e5-5e37-f971-e7ad-c4db04781d2f/Cdk1JcZ343w5S4fdcTYm7rBs9X91usVNe_wKpKCDuFV3O0oapFpozXSN2g) or review the provided PDF file in the repository's root directory.
