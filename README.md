# Melanoma Detection Assignment
Melanoma is the deadliest type of skin cancer, accounting for 75% of skin cancer deaths. Early detection significantly increases treatment success. This project aims to build a CNN-based automated classification system to detect melanoma from skin lesion images. By leveraging image augmentation and deep learning techniques, the model reduces manual diagnosis efforts and improves predictive accuracy.

## Problem Statement
To develop a Convolutional Neural Network (CNN) model that accurately detects melanoma using dermatoscopic images. The solution alerts dermatologists to the presence of melanoma, enhancing early diagnosis and saving lives.

## Table of Contents
•⁠  ⁠[General Info](#general-info)
•⁠  ⁠[Model Architecture](#model-architecture)
•⁠  ⁠[Model Summary](#model-summary)
•⁠  ⁠[Model Evaluation](#model-evaluation)
•⁠  ⁠[Technologies Used](#technologies-used)
•⁠  ⁠[Acknowledgements](#acknowledgements)
•⁠  ⁠[Collaborators](#collaborators)

## General Info
The dataset contains *2,357 dermatoscopic images* categorized into benign and malignant classes. To address class imbalance, the *Augmentor* library was used for data augmentation, ensuring balanced class representation.


![image](https://github.com/user-attachments/assets/91830de7-fae5-4a1a-bcba-1acb6bae96b2)


## Model Architecture
The CNN model comprises the following steps:
1.⁠ ⁠*Data Augmentation*: Random transformations (rotation, scaling, flipping) to enhance diversity.
2.⁠ ⁠*Normalization*: Scaling pixel values to [0, 1] using ⁠ Rescaling(1./255) ⁠.
3.⁠ ⁠*Convolutional Layers*: Three ⁠ Conv2D ⁠ layers (16, 32, 64 filters) with ReLU activation and max pooling.
4.⁠ ⁠*Dropout*: Applied to prevent overfitting.
5.⁠ ⁠*Flattening & Fully Connected Layers*: Dense layers (128 neurons) for feature learning.
6.⁠ ⁠*Output Layer*: Final layer for classification.
7.⁠ ⁠*Optimization: Compiled using **Adam Optimizer* and ⁠ SparseCategoricalCrossentropy ⁠ loss.

## Model Summary

![image](https://github.com/user-attachments/assets/e1d1173b-eb62-469d-84b1-7ae41483e18a)


## Model Evaluation

Training accuracy improved steadily to *88.91%, with validation accuracy reaching **94.81%, indicating minimal overfitting. Techniques like **class rebalancing, augmentation, Dropout, and **Batch Normalization* significantly enhanced performance.

![image](https://github.com/user-attachments/assets/6a627f22-663f-4660-aa81-f73b67a447dd)


## Technologies Used
•⁠  ⁠*Python* - version 3.10.13
•⁠  ⁠*TensorFlow* - version 2.13.1
•⁠  ⁠*NumPy* - version 1.24.3
•⁠  ⁠*Pandas* - version 2.2.3
•⁠  ⁠*Matplotlib* - version 3.7.1
•⁠  ⁠*Seaborn* - version 0.12.2

## Acknowledgements
•⁠  ⁠[Melanoma Skin Cancer Information](https://www.cancer.org/cancer/melanoma-skin-cancer/about/what-is-melanoma.html)
•⁠  ⁠Tutorials on CNN and Deep Learning from UpGrad and Towards Data Science.

## Collaborators
Created by (https://github.com/thomami244).
