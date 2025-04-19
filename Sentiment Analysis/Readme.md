# Sentiment Analysis System

## Overview
This project implements a sentiment analysis system that classifies movie reviews as either positive (1) or negative (0). The system utilizes deep learning techniques including LSTM (Long Short-Term Memory) and GRU (Gated Recurrent Unit) networks to analyze text sentiment.

## Dataset
The project uses the IMDB movie review dataset, which includes:

25,000 movie reviews labeled by sentiment (positive/negative).
After preprocessing, the reviews encoded as sequences of word indexes (integers).

## Technical Details
Optimizer: Adam
Loss Function: Binary Cross-Entropy
Batch Size: 32
Training Epochs: 3
Sequence Length: Limited to 100 words per review
Vocabulary Size: 20,000 most frequent words

## Model Architecture
Two separate models were implemented and compared:

### LSTM Model
Input Layer: Word sequences (max length: 100)
Embedding Layer: 128-dimensional word embeddings
LSTM Layer: 128 units
Dropout Layer: 0.4 dropout rate
Output Layer: Dense layer with sigmoid activation

### GRU Model
Input Layer: Word sequences (max length: 100)
Embedding Layer: 128-dimensional word embeddings
GRU Layer: 128 units
Dropout Layer: 0.4 dropout rate
Output Layer: Dense layer with sigmoid activation

## Results

### LSTM Model:
Accuracy: 80%
Loss: 0.73

### GRU Model:
Accuracy: 84%
Loss: 0.43

The GRU model outperformed the LSTM model in both accuracy and loss metrics.

