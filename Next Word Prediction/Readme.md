# Next Word Prediction

## Overview
Next Word Prediction is a deep learning project that creates a language model capable of predicting the next word in a given text sequence. Using recurrent neural networks (RNNs) and Long Short-Term Memory (LSTM) networks, the model learns patterns and relationships from text data to make accurate predictions.

## Features
Text preprocessing and tokenization.
Sequence generation for training data.
Deep learning model with dual LSTM layers.
Streamlit web application for user-friendly interaction.

## Dataset
The model is currently trained on the complete text of Jane Austen's "Pride and Prejudice."

## Model Architecture
The neural network consists of:
Embedding layer (input dimension: vocabulary size, output dimension: 10)
Two LSTM layers (1000 units each)
Dense layer with ReLU activation (1000 units)
Output layer with softmax activation (vocabulary size units)

## Technical Details
Model Type: Sequential with stacked LSTM
Tokenization: Keras Tokenizer
Optimizer: Adam (learning rate: 0.001)
Loss Function: Categorical Cross-Entropy
Batch Size: 64
Training Epochs: 70
