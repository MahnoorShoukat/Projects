# Wildfire Detection System

## Overview
This project implements a Convolutional Neural Network (CNN) to detect wildfires in images. The system preprocesses noisy input images to enhance quality and improve detection accuracy. The model is trained on a dataset of fire and non-fire images to classify whether an image contains a wildfire.

## Dataset Structure
The dataset should be organized as follows:
forest_fire/
├── Training and Validation/
│   ├── fire/
│   └── nofire/
└── Testing/
    ├── fire/
    └── nofire/

## Model Architecture
Input: RGB images (150x150x3)
4 Convolutional layers with MaxPooling
Flatten layer
Dense layer with 512 units and ReLU activation
Dropout layer (15%)
Output layer with sigmoid activation for binary classification

## Training Process
Images are rescaled to values between 0 and 1
Batch size of 32 is used for training
Adam optimizer with binary cross-entropy loss
Early stopping mechanism to prevent overfitting
Model checkpointing to save the best weights

## Performance Visualization
The training history includes loss and validation loss curves to visualize model performance and identify potential overfitting.

## Model Evaluation
Accuracy is measured on both the training and test datasets. The final model predicts binary labels (1 for "No Fire", 0 for "Fire").
