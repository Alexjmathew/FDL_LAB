Image Classification on CIFAR-10 using Neural Networks
Aim

To implement a Python program for the classification of images in the CIFAR-10 dataset using a neural network.

Algorithm

    Load the CIFAR-10 dataset, which contains 60,000 32x32 color images in 10 different classes and split the dataset into training and testing sets.

    Normalize pixel values to be between 0 and 1. Convert labels to one-hot encoding.

    Define a neural network model with a flatten layer and three dense layers with specified hidden units and activation function.

    Compile the model with Adam optimizer, categorical crossentropy loss, and accuracy metric.

    Train the model on the training data for 5 epochs.

    Evaluate the model on the test data and store the test accuracy.

    Store relevant information about the model (hidden units, activation, test accuracy) in a dictionary.

    Display information about each run and the run with the highest test accuracy.

    Make predictions on a few sample images and plot a probability meter.


This project implements a neural network for classifying images from the CIFAR-10 dataset. The CIFAR-10 dataset consists of 60,000 32x32 color images in 10 different classes, with 6,000 images per class. The goal is to build and train a neural network model that can accurately classify these images.
Dataset

The CIFAR-10 dataset contains images in the following 10 classes:

    Airplane

    Automobile

    Bird

    Cat

    Deer

    Dog

    Frog

    Horse

    Ship



    Truck
