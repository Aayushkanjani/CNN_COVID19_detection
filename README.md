# CNN_COVID19_detection
This repository contains the implementation of a Convolutional Neural Network (CNN) model for detecting COVID-19 from chest X-ray images using the EfficientNetB1 pre-trained model.


## Table of Contents

- [Introduction](#introduction)
- [Dataset](#dataset)
- [Model Architecture](#model-architecture)
- [Training](#training)
- [Evaluation](#evaluation)
- [Results](#results)


## Introduction

The COVID-19 pandemic has highlighted the need for rapid and accurate diagnostic tools. This project leverages deep learning, specifically a Convolutional Neural Network (CNN), to identify COVID-19 infection from chest X-ray images. The model is built on the EfficientNetB1 architecture, which is known for its efficiency and performance on image classification tasks.

## Dataset

The dataset used for training and evaluation includes chest X-ray images labeled as COVID-19 positive, pneumonia, and normal. The dataset can be downloaded from [Kaggle's COVID-19 Radiography Database](https://www.kaggle.com/tawsifurrahman/covid19-radiography-database).

## Installation

Clone this repository to your local machine:


git clone https://github.com/aayushkanjani/CNN_COVID19_detection.git
cd CNN_COVID19_detection

## Model Architecture
The model uses the EfficientNetB1 pre-trained model as the base. The architecture includes:

EfficientNetB1 base model (pre-trained on ImageNet)
Global average pooling layer
Fully connected layer with dropout for regularization
Output layer with softmax activation for classification


## Training
The model is trained using the following settings:

Optimizer: Adamax
Loss function: Categorical Crossentropy
Metrics: Accuracy
Number of epochs: 25 (can be adjusted)
Batch size: 32 (can be adjusted)

## Evaluation
The model is evaluated on a separate test set. Evaluation metrics include accuracy and confusion matrix.

## Results
The model achieved an accuracy score of 95.37% on the test data.
