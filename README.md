# 🏛️ Landmark Recognition Using Deep Learning

<p align="center">
  <img src="https://img.shields.io/badge/Deep%20Learning-Landmark%20Recognition-blue?style=for-the-badge" alt="Deep Learning">
  <img src="https://img.shields.io/badge/Python-3.x-yellow?style=for-the-badge&logo=python" alt="Python">
  <img src="https://img.shields.io/badge/TensorFlow-2.x-orange?style=for-the-badge&logo=tensorflow" alt="TensorFlow">
  <img src="https://img.shields.io/badge/EfficientNetB0-Transfer%20Learning-green?style=for-the-badge" alt="EfficientNetB0">
  <img src="https://img.shields.io/badge/Google%20Colab-Notebook-red?style=for-the-badge&logo=googlecolab" alt="Google Colab">
</p>

<p align="center">
  <b>AI-powered image classification system for recognizing famous landmarks using Deep Learning and Transfer Learning.</b>
</p>

---

## 📌 Project Overview

**Landmark Recognition Using Deep Learning** is a computer vision project designed to identify and classify famous landmarks from images.

The project uses a **pre-trained EfficientNetB0 model** with **Transfer Learning** to extract meaningful visual features from landmark images and classify them into different landmark categories.

The complete pipeline includes:

- Dataset exploration
- Class distribution analysis
- Landmark image visualization
- Train-validation splitting
- Image preprocessing
- Data augmentation
- Transfer learning
- Model training
- Performance evaluation
- Confusion matrix analysis
- Real-image prediction

The trained model can also accept a new landmark image and predict the corresponding landmark class along with its confidence score.

---

# 🎯 Project Objectives

The main objectives of this project are:

1. To build an image classification system for landmark recognition.
2. To understand and implement a complete Deep Learning workflow.
3. To explore and visualize a landmark image dataset.
4. To apply image preprocessing and augmentation techniques.
5. To use Transfer Learning with EfficientNetB0.
6. To train a Deep Learning classification model.
7. To evaluate the model using multiple performance metrics.
8. To analyze classification errors using a confusion matrix.
9. To predict landmarks from unseen images.
10. To understand the practical implementation of Computer Vision.

---

# 🧠 Problem Statement

Recognizing landmarks from images can be challenging because different landmarks may have similar architectural structures, colors, shapes, backgrounds, and viewpoints.

Traditional image-processing techniques require manually designed features and may not generalize well to different images.

This project solves the problem using **Deep Learning**, where a pre-trained convolutional neural network automatically learns powerful visual features and classifies images into their corresponding landmark categories.

---

# 💡 Proposed Solution

The proposed system uses **EfficientNetB0**, a lightweight and efficient convolutional neural network pre-trained on ImageNet.

Instead of training a deep neural network completely from scratch, the project uses the knowledge learned from ImageNet and adds a custom classification layer for the landmark dataset.

### Workflow

```text
                 ┌─────────────────────┐
                 │   Landmark Dataset  │
                 └──────────┬──────────┘
                            │
                            ▼
                 ┌─────────────────────┐
                 │ Dataset Exploration │
                 └──────────┬──────────┘
                            │
                            ▼
                 ┌─────────────────────┐
                 │ Image Preprocessing │
                 └──────────┬──────────┘
                            │
                            ▼
                 ┌─────────────────────┐
                 │ Data Augmentation   │
                 └──────────┬──────────┘
                            │
                            ▼
                 ┌─────────────────────┐
                 │   EfficientNetB0    │
                 │ Pre-trained Model   │
                 └──────────┬──────────┘
                            │
                            ▼
                 ┌─────────────────────┐
                 │ Global Avg Pooling  │
                 └──────────┬──────────┘
                            │
                            ▼
                 ┌─────────────────────┐
                 │      Dropout        │
                 └──────────┬──────────┘
                            │
                            ▼
                 ┌─────────────────────┐
                 │ Softmax Classifier  │
                 └──────────┬──────────┘
                            │
                            ▼
                 ┌─────────────────────┐
                 │ Landmark Prediction │
                 └─────────────────────┘

