# MNIST CNN Image Classification

A Convolutional Neural Network (CNN) based image classification project using the MNIST handwritten digit dataset.

## Overview

This project demonstrates the basic workflow of image classification using a CNN:

- Loading and preparing the MNIST dataset
- Exploring convolution and padding concepts
- Building a CNN model
- Training the model on handwritten digit images
- Evaluating the trained model
- Visualizing predictions on test images
- Performing inference on an external image

## Dataset

The project uses the **MNIST handwritten digit dataset**, which contains grayscale images of handwritten digits from 0 to 9.

Each image belongs to one of 10 classes:

`0, 1, 2, 3, 4, 5, 6, 7, 8, 9`

## CNN Workflow

The notebook covers the following workflow:

```text
MNIST Dataset
      ↓
Data Preparation
      ↓
CNN Model
      ↓
Training
      ↓
Evaluation
      ↓
Test Image Prediction
      ↓
External Image Inference


Padding Demonstration

The notebook also demonstrates the effect of different padding approaches in convolutional layers, including valid and same padding.

This was included to understand how padding affects the spatial dimensions of feature maps.

Model Training

A CNN model is trained on the MNIST dataset for handwritten digit classification.

The model uses convolutional layers for feature extraction followed by fully connected layers for classification into the 10 digit classes.

Evaluation and Prediction

After training, the model is evaluated and tested on images from the MNIST test set.

Individual test images are also passed through the model to compare:

True label
Predicted label
Prediction confidence
External Image Inference

An inference pipeline was implemented to accept an external handwritten-digit image.

The image is processed before prediction by:

Converting the image to grayscale
Inverting the image when required
Resizing it to the model's expected input size
Normalizing pixel values
Preparing the image tensor for the CNN
Passing the processed image to the trained model

The model then returns the predicted digit and its confidence.

Learning Outcome

This project was used to understand the practical workflow of CNN-based image classification, from dataset preparation and model training to evaluation and inference on an external image.

Note

The external-image inference is an experimental learning step. The model may perform differently on images that differ from the MNIST training data in handwriting style, image format, positioning, or preprocessing.

Project Structure

├── README.md
└── MNIST_CNN_Image_Classification.ipynb


