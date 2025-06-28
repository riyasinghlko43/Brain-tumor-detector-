# 🧠 Brain Tumor Detection using CNN

This project uses Convolutional Neural Networks (CNN) to detect the presence of brain tumors in MRI scans. The model classifies images into two categories: **Tumor** and **No Tumor**. It’s built using Python, TensorFlow/Keras, and OpenCV.

---

## 📌 Table of Contents

- [Overview](#overview)
- [Dataset](#dataset)
- [Model Architecture](#model-architecture)
- [Installation](#installation)
- [How to Run](#how-to-run)
- [Results](#results)
- [Future Scope](#future-scope)
- [Contributors](#contributors)

---

## 🧾 Overview

Brain tumors are a serious health issue, and early detection is crucial. This project automates tumor detection from MRI scans using deep learning techniques. The CNN model is trained on a labeled dataset and tested for real-world performance.

---

## 📂 Dataset

The dataset contains brain MRI images categorized as:

- **yes/** – Images with brain tumors
- **no/** – Images without brain tumors

> Total images: ~3000+

The dataset is loaded and preprocessed using OpenCV and TensorFlow.

---

## 🧠 Model Architecture

The CNN model has the following layers:

- 3 Convolutional + MaxPooling layers
- Flatten layer
- Dense layer (ReLU)
- Output layer (Sigmoid for binary classification)

Compiled with:
```python
loss='binary_crossentropy'
optimizer='adam'
metrics=['accuracy']
