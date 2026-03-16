# Brain Tumor Classification using CNN and Transfer Learning

Deep learning model for automatic brain tumor classification from MRI images using a Convolutional Neural Network (CNN) and transfer learning with the VGG16 architecture.

---

## Project Overview

Brain tumor classification from MRI images is an important task in medical image analysis and computer-aided diagnosis.

The goal of this project is to develop a deep learning model capable of automatically classifying brain MRI images into four categories:

* Glioma
* Meningioma
* Pituitary tumor
* No tumor

The model uses transfer learning to leverage previously learned visual features from large image datasets and adapt them to the medical imaging domain.

---

## Dataset

The dataset consists of brain MRI images obtained from a public dataset on Kaggle.

Classes included in the dataset:

* Glioma
* Meningioma
* Pituitary tumor
* No tumor

The dataset was divided into training and testing sets to evaluate the model’s performance.

---

## Image Preprocessing

Before training the model, several preprocessing techniques were applied:

* Image resizing to **224 × 224 pixels**
* Normalization using `preprocess_input()` from the VGG16 module
* Conversion of images to the format expected by the pre-trained network

---

## Data Augmentation

To improve model generalization and reduce overfitting, **data augmentation** techniques were applied:

* Random rotation
* Zoom
* Horizontal flipping
* Horizontal and vertical shifts

These transformations were implemented using `ImageDataGenerator`.

---

## Model Architecture

The model is based on **Transfer Learning** using the VGG16 architecture pre-trained on ImageNet.

Key steps:

1. Load VGG16 without the fully connected top layers
2. Freeze convolutional layers to preserve learned visual features
3. Add custom dense layers for classification
4. Train the final layers on the MRI dataset

This approach allows the model to perform well even with a relatively limited medical dataset.

---

## Training Configuration

* Optimizer: **Adam**
* Loss function: **categorical_crossentropy**
* Batch size: **32**
* Epochs: **20**
* EarlyStopping used to prevent overfitting

---

## Results

The model achieved an overall accuracy of:

**Accuracy: 92%**

Evaluation metrics such as **precision, recall and F1-score** show strong performance across all tumor classes.

This demonstrates the effectiveness of convolutional neural networks for medical image classification tasks.

---

## Technologies Used

* Python
* TensorFlow / Keras
* NumPy
* Matplotlib
* Google Colab

---

## Project Structure

brain-tumor-classification-cnn

* brain_tumor_classification.ipynb
* project_presentation.pdf
* README.md

---

## Author

**Ana Laura Della Rosa**

Biomedical Engineer interested in Artificial Intelligence, Machine Learning and medical imaging applications.

