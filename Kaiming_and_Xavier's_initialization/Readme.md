Aim

To implement a python program to compare the impact of Kaiming and Xavier weight initialization techniques, regularization and dropout on a neural network's performance during training and validation using the CIFAR-10 dataset.
Algorithm

    Import necessary libraries and load CIFAR-10 Dataset. Normalize the pixel values to the range [0, 1].

    Create a function (create_model) to build a neural network model. The model has a flattening layer followed by multiple dense layers with specified configurations (number of units, activation function, initializers, regularization).

    Initialize weights using Xavier/Glorot and Kaiming/He initializers.

    Compile models using the Adam optimizer, categorical crossentropy loss, and accuracy as a metric.

    Train both models with specified configurations and store the training history.

    Evaluate and visualize the performance of the models using training and validation accuracy over epochs.

    Plot and display the training and validation accuracy for both models.

Files

    Kaiming_and_Xavier's_initialization.ipynb: Main Python script containing the implementation

    README.md: This documentation file
