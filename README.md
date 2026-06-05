# Industrial Surface Crack Detection using CNN

## Overview

This project implements a Convolutional Neural Network (CNN) for automated industrial surface crack detection. The model classifies surface images into two categories:

* Crack
* No Crack

The system performs data preprocessing, image augmentation, CNN training, model evaluation, and single-image prediction.

## Features

* Image preprocessing and normalization
* Data augmentation
* CNN-based binary classification
* Batch Normalization and Dropout
* Early Stopping and Learning Rate Reduction
* Confusion Matrix and Classification Report
* Single image prediction support

## Tech Stack

* Python
* TensorFlow / Keras
* NumPy
* Matplotlib
* Scikit-Learn

## Dataset Structure

CrackDataset/

├── Positive/

└── Negative/

Positive folder contains crack images.

Negative folder contains non-crack images.

## CNN Architecture

* Conv2D (32 Filters)

* BatchNormalization

* MaxPooling

* Conv2D (64 Filters)

* BatchNormalization

* MaxPooling

* Conv2D (128 Filters)

* BatchNormalization

* MaxPooling

* Conv2D (256 Filters)

* BatchNormalization

* MaxPooling

* Dense (256)

* Dropout (0.5)

* Dense (128)

* Dropout (0.3)

* Output Layer (Sigmoid)

## Model Training

* Optimizer: Adam
* Loss Function: Binary Crossentropy
* Metric: Accuracy
* Early Stopping
* Model Checkpoint
* ReduceLROnPlateau

## Results

The model successfully detects cracks from industrial surface images and provides predictions on unseen test data.

Performance evaluation includes:

* Test Accuracy
* Confusion Matrix
* Classification Report

## Project Structure

Industrial-Surface-Crack-Detection-CNN/

├── Crack_Detection_CNN.py

├── README.md

├── requirements.txt

├── Sample_Results/

│ ├── accuracy_graph.png

│ ├── loss_graph.png

│ └── confusion_matrix.png

└── Saved_Model/

└── Best_Crack_Detection_Model.keras

## Installation

pip install -r requirements.txt

## Run Project

python Crack_Detection_CNN.py

## Author

Siddhi Kakade

Final Year Computer Engineering

AI/ML Enthusiast

