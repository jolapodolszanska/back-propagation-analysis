The program includes a function `generate_dataset(N_points)` that generates a dataset consisting of two classes distributed around a circle with varying radii:
- Class 1: elements are closer to the center.
- Class 0: elements are further from the center.

For data visualization, the *matplotlib* library is used. Initial weights for the neural network are defined using random values for weights `w1, w2` and zeros for biases `b1, b2`. Two functions are used for forward and backward propagation:
- The function `forward_propagation(X, weights)` calculates the network's predictions based on the input data and current weights,
- The function `back_propagation(X, Y_T, weights)` uses the results from forward propagation to calculate weight gradients through backward error propagation. This is the core of the learning algorithm.

The network is trained over a specified number of epochs, updating weights based on the calculated gradients while simultaneously recording the values of the loss function. After training, a visualization of the training is generated. An option to overlay training data on decision maps has been added, which helps to better understand how the model handles data classification. Additionally, a new dataset simulating the XOR problem is generated, and the model is retrained on these data. This demonstrates how the model handles more complex, non-linearly separable problems.

This code demonstrates a comprehensive approach to building and training simple neural networks in Python. It teaches the network how to recognize patterns in data and classify them based on the learned decision boundary. The program is well-organized and covers all stages of the machine learning process from data generation, through model training, to evaluation and visualization of results.
<p align="center">
Distribution of class data
</p>

<p align="center">
<img src="https://raw.githubusercontent.com/jolapodolszanska/back-propagation-analysis/main/img/Figure%202024-07-29%20115103%20(0).png" />
</p>

<p align="center">
  Training loss curve
</p>

<p align="center">
<img src="https://raw.githubusercontent.com/jolapodolszanska/back-propagation-analysis/main/img/Figure%202024-07-29%20115103%20(1).png" />
</p>
