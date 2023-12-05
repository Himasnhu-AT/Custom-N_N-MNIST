# Custom Neural Network for MNIST Number Prediction

This repository, named Custom-N_N-MNIST, houses a custom neural network tailored for predicting numerical values from the MNIST dataset. For a detailed explanation and walkthrough, please refer to the [Evernote document](https://www.evernote.com/shard/s560/sh/df35c6e5-5e37-f971-e7ad-c4db04781d2f/Cdk1JcZ343w5S4fdcTYm7rBs9X91usVNe_wKpKCDuFV3O0oapFpozXSN2g) or access the PDF file located in the repository's root directory.

## Overview

The neural network begins with the preprocessing of image data, transforming it into a 28 x 28 format, resulting in an image output represented by 784 bits. The dataset is structured as a matrix of size 784 x n, where n corresponds to the number of images. The architecture of the neural network consists of an initial/input layer (a0) with 784 nodes, two hidden layers (z1 and z2) each containing 10 nodes, and a final output layer.

## Activation Functions

- **ReLU (Rectified Linear Unit):** Applied as the activation function for the hidden layers.
- **Softmax Activation:** Employed on the output layer to convert raw scores into probabilities for each digit class.

## Training the Neural Network

The network parameters are randomly initialized, and gradient descent is utilized for optimization. The training process involves forward and backward propagation to compute gradients and iteratively update weights and biases. The script prints the accuracy of predictions every 10 iterations.

## Testing and Visualization

The trained neural network is tested on a few samples from the training set. Additionally, the script includes a function (`test_prediction`) to visualize predictions for specific images in the training set.

## Usage

1. **Loading Data:** Replace the empty string in `pd.read_csv('')` with the path to your MNIST dataset.

2. **Training:** Adjust hyperparameters, such as learning rate (`alpha`) and the number of iterations, as needed. The `gradient_descent` function trains the neural network.

3. **Testing and Visualization:** Use the `test_prediction` function to visualize predictions for specific indices in the training set.

4. **Evaluation:** Evaluate the model's accuracy on a validation set (`X_dev`, `Y_dev`) after training.

Feel free to experiment with the code, tweak parameters, and visualize predictions to gain insights into the working of this custom neural network for MNIST digit recognition.

## Dependencies

- NumPy
- Pandas
- Matplotlib

Make sure to install these dependencies before running the code.

## Accessing the Explanation

For a comprehensive explanation of the neural network's development and operation, please visit the [Evernote document](https://www.evernote.com/shard/s560/sh/df35c6e5-5e37-f971-e7ad-c4db04781d2f/Cdk1JcZ343w5S4fdcTYm7rBs9X91usVNe_wKpKCDuFV3O0oapFpozXSN2g) or review the provided PDF file in the repository's root directory.
