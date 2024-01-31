# Rock-Paper-Scissors Image Classifier

This repository contains a TensorFlow-based deep learning project aimed at classifying images of hand gestures into three categories: Rock, Paper, or Scissors. Using Convolutional Neural Networks (CNNs) within the Keras API, the model is adept at recognizing and categorizing gestures from visual data.

## Model Overview

- **Framework**: TensorFlow 2.15.0
- **API**: Keras
- **Model Architecture**: Convolutional Neural Network (CNN)

### Architecture Details:
- **Feature Extraction Layers**: Conv2D layers with ReLU activation.
- **Downsampling Layers**: MaxPooling2D layers.
- **Classification Layers**: Dense layers with ReLU activation.
- **Regularization**: Dropout layers and L2 regularization to mitigate overfitting.
- **Output Layer**: Dense layer with Softmax activation for multi-class classification.

## Dataset Information

- **Source**: [Dicoding Academy](https://github.com/dicodingacademy/assets/releases/download/release/rockpaperscissors.zip)
- **Contents**: Hand gesture images representing Rock, Paper, and Scissors.
- **Split**:
  - Training set: 1,312 images
  - Validation set: 876 images

## Model Performance

- **Optimization**: Adam optimizer with a custom learning rate schedule.
- **Regularization Techniques**: L2 regularization and Dropout.
- **Best Validation Loss**: 0.26198
- **Best Validation Accuracy**: 96.58%

## Features

- **Data Augmentation**: Implemented to introduce variability in the training dataset, enhancing model robustness.
- **Learning Rate Scheduling**: Applied to optimize convergence rates.
- **Early Stopping and Model Checkpointing**: Utilized to halt training at the optimal point and save the best model iteration, respectively.
- **Comprehensive Evaluation**: Both training and validation metrics are extensively monitored to gauge model performance.
