#Convolutional Neural Network for MNIST Classification

This repository contains a simple convolutional neural network (CNN) model implemented using TensorFlow and Keras to classify images from the MNIST dataset. The MNIST dataset consists of 70,000 grayscale images of handwritten digits with a size of 28x28 pixels. The images are split into 60,000 training samples and 10,000 testing samples.

The model architecture consists of two convolutional blocks followed by two fully connected (dense) layers. Each convolutional block consists of two convolutional layers with batch normalization and ReLU activation followed by max pooling and dropout. The first convolutional block has 32 filters with a kernel size of 5x5 and the second block has 64 filters with a kernel size of 3x3. The fully connected layers consist of 256 and 10 neurons respectively, with dropout applied to the first dense layer to reduce overfitting. The model is trained using categorical cross-entropy loss and optimized using the Adam optimizer.

To improve the model's generalization ability and prevent overfitting, an image data generator is used to augment the training data by randomly rotating, zooming, and shifting the images. An early stopping callback is used during training to stop the training process if the validation loss doesn't improve after 5 epochs.

##Getting Started
###Prerequisites
Python 3.x
TensorFlow 2.x
Keras
NumPy
Matplotlib

##Results
The model achieves an accuracy of approximately 99.54% on the test set after training for 33 epochs.

