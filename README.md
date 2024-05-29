# Audio Classification Project

This project focuses on preprocessing audio data and creating a machine learning model to classify different types of sounds using the UrbanSound8K dataset.

## Table of Contents
- [Introduction](#introduction)
- [Dataset](#dataset)
- [Dependencies](#dependencies)
- [Project Structure](#project-structure)
- [Data Preprocessing](#data-preprocessing)
- [Model Creation](#model-creation)
- [Training](#training)
- [Evaluation](#evaluation)

## Introduction
The goal of this project is to build a model that can classify audio samples into different categories. This is achieved by extracting features from the audio files and training a neural network.

## Dataset
The dataset used in this project is the UrbanSound8K dataset, which contains 8,732 labeled sound excerpts (<=4s) of urban sounds from 10 classes.

## Dependencies
To run this project, you need the following libraries:
- pandas
- numpy
- librosa
- matplotlib
- tensorflow
- sklearn
- keras

You can install the required dependencies using the following commands:
```bash
pip install pandas numpy librosa matplotlib tensorflow sklearn keras
```
## Project Structure
The project consists of the following main components:

- **Data Preprocessing:** Feature extraction from audio files.
- **Model Creation:** Building and compiling the neural network.
- **Training:** Training the model with the training dataset.
- **Evaluation:** Evaluating the model's performance on the test dataset.

## Data Preprocessing
The data preprocessing steps include loading audio files, extracting MFCC features, and scaling the features.

## Model Creation
A Sequential neural network model is created using Keras with the following architecture:

- Input layer with 100 neurons
- Hidden layers with 200 and 100 neurons
- Output layer with softmax activation

## Training
The model is trained using categorical crossentropy loss and Adam optimizer. A checkpoint callback is used to save the best model.

## Evaluation
The model's performance is evaluated on the test dataset, and the accuracy is printed.

