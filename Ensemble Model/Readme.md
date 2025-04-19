# Fashion Recommendation System Using Ensemble Learning

## Overview
This project implements an ensemble learning approach to predict clothing recommendations based on a variety of attributes. By combining multiple machine learning algorithms, the system achieves robust prediction performance with an accuracy of 81%.

## Dataset
The model uses the "Attribute DataSet.csv" from Kaggle, which contains various clothing attributes such as:
Style
Price
Rating
Size
Season
NeckLine
SleeveLength
Waiseline
Material
FabricType
Decoration
Pattern Type

## Data Preprocessing
Handling missing values using mean imputation

### Feature engineering
Created some new columns.
Categorical variable encoding using one-hot encoding.
Feature scaling with StandardScaler.
Feature extraction using Linear Discriminant Analysis (LDA).

## Model Architecture
Base Learners
- Random Forest Classifier
- XGBoost Classifier
- Artificial Neural Network (MLP Classifier)

Meta Learner
- Multi-Layer Perceptron Classifier (ANN)

## Evaluation Method
K-fold cross-validation with various k values (2, 3, 4, 6)

## Performance metrics
Accuracy
Precision
Recall
Confusion Matrix

## Results
The ensemble approach significantly outperforms individual models with an overall accuracy of 81%.