# Air Quality Prediction System

## Overview
This project predicts air quality based on various pollutant measurements. It calculates different sub-indices for major air pollutants (SO2, NO2, RSPM, SPM), determines the overall Air Quality Index (AQI), and classifies the air quality into categories ranging from "Good" to "Hazardous". The system includes a machine learning model (K-Nearest Neighbors) to predict air quality classification and provides an interactive Streamlit web interface for real-time predictions.

## Dataset
The dataset contains air quality measurements from various monitoring stations, including:
Location and monitoring station information
State information
Pollutant measurements: SO2, NO2, RSPM (PM10), SPM
Station type (e.g., Industrial, Residential)

## Data Preprocessing
Handling missing values in categorical features using mode imputation
Filling numerical missing values appropriately
Removing unnecessary columns

## Feature Engineering
Calculation of sub-indices for each pollutant according to standard AQI formulas:
SO2 Index (SOi)
NO2 Index (NOi)
Respirable Suspended Particulate Matter Index (RPi)
Suspended Particulate Matter Index (SPMi)

## Modeling
Algorithm: K-Nearest Neighbors Classifier
Training/Testing Split: 67% training, 33% testing
Evaluation Metrics: Accuracy, Kappa Score
Model Serialization: Saved as 'Trained_model.sav'

