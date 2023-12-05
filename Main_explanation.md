# Explanation of Digit Recognition Neural Network

This Python code implements a simple neural network for digit recognition using the Kaggle Digit Recognizer dataset. The neural network has one hidden layer with ReLU activation and uses softmax for the output layer.

## Dataset
The dataset for digit recognition can be found [here](https://www.kaggle.com/competitions/digit-recognizer). Ensure that the dataset is downloaded and the path is correctly specified in the code.

## Code Overview

### Data Preprocessing
- Load the dataset using pandas and convert it to a NumPy array.
- Shuffle the data randomly.
- Split the dataset into a development set (`data_dev`) and a training set (`data_train`).

### Neural Network Architecture
- Initialize the neural network parameters (weights and biases) using the `init_params` function.
- Implement the ReLU activation function (`ReLU`) and softmax activation function (`softmax`).
- Define the forward propagation function (`forward_prop`) to compute the output of the neural network.
- Implement the backward propagation function (`backward_prop`) to calculate gradients for the parameters.
- Update the parameters using the gradient descent optimization algorithm with the `update_params` function.

### Training the Neural Network
- Use the `gradient_descent` function to train the neural network on the training set (`X_train` and `Y_train`).
- Display the accuracy on the training set at every 10 iterations.

### Making Predictions
- Implement the `make_predictions` function to obtain predictions for a given input using the trained parameters.
- Visualize and test predictions using the `test_prediction` function on a few examples from the training set.

### Evaluation on Development Set
- Make predictions on the development set (`X_dev`) using the trained parameters.
- Evaluate the accuracy of the predictions on the development set using the `get_accuracy` function.

## Execution
To run the code, ensure that the Kaggle Digit Recognizer dataset is downloaded, and the path is correctly specified. The neural network is trained using gradient descent with specified learning rate (`alpha`) and number of iterations (`500` in this case). After training, predictions are made on the development set, and a few examples from the training set are visualized along with their predictions and labels.

Note: This code is a basic implementation, and further optimizations can be applied to improve the model's performance.
