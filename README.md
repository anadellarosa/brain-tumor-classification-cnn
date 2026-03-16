# Brain Tumor Classification using CNN and Transfer Learning

This project implements a deep learning model for automatic classification of brain tumors using MRI images.

The model is based on transfer learning using the VGG16 architecture pre-trained on ImageNet.

## Problem

Brain tumor classification from MRI images is an important task in medical image analysis and computer-aided diagnosis.

The objective of this project is to automatically classify MRI images into four categories:

- Glioma
- Meningioma
- Pituitary tumor
- No tumor

## Dataset

MRI images dataset obtained from Kaggle.

Classes:
- Glioma
- Meningioma
- Pituitary
- No tumor

## Model

Transfer Learning with VGG16.

Steps:
1. Image preprocessing
2. Data augmentation
3. Feature extraction using VGG16
4. Custom classification layers
5. Training and evaluation

## Training configuration

- Optimizer: Adam
- Loss function: categorical_crossentropy
- Batch size: 32
- Epochs: 20
- EarlyStopping used to avoid overfitting

## Results

Accuracy: **92%**

The model shows strong performance across all classes using precision, recall and F1-score metrics.

## Technologies

- Python
- TensorFlow / Keras
- NumPy
- Matplotlib
- Google Colab

## Authors

Ana Laura Della Rosa  
Biomedical Engineer interested in AI and Machine Learning for healthcare.
