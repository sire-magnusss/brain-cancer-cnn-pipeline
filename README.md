# Brain Cancer MRI Classification Pipeline

[![Notebook on Kaggle](https://img.shields.io/badge/Kaggle-Notebook-orange)](https://www.kaggle.com/datasets/orvile/brain-cancer-mri-dataset)  
[![License](https://img.shields.io/badge/License-Apache-green)](LICENSE)

---

## 🚀 Overview

This project implements a **state-of-the-art** convolutional neural network (CNN) pipeline for **multi-class** brain cancer detection from MRI scans. Leveraging real-time data augmentation, hyperparameter optimization (Keras Tuner Hyperband), and thorough evaluation metrics, we achieve **>94% validation accuracy** on the Orvile Brain Cancer MRI dataset.  

> **Impact:** Early and accurate detection of brain tumors can significantly improve patient outcomes. This open-source pipeline offers researchers and clinicians a turnkey solution to train, evaluate, and deploy high-accuracy diagnostic models.

---

## 📋 Table of Contents

1. [Features](#features)  
2. [Dataset](#dataset)  
3. [Getting Started](#getting-started)  
4. [Pipeline Structure](#pipeline-structure)  
5. [Results](#results)  
6. [Usage](#usage)  
7. [Future Directions](#future-directions)  
8. [License](#license)  
9. [References](#references)

---

## ✨ Features

- **Data Loading & Visualization**  
  - Automatic directory traversal into `glioma`, `meningioma`, `pituitary`, and `no_tumor` classes  
  - Class balance barplots and sample image previews  

- **Augmentation & Preprocessing**  
  - Rotation, translation, shear, zoom, and flipping to simulate real-world MRI variations  

- **Hyperparameter Optimization**  
  - Keras Tuner Hyperband search over CNN architecture (filters, dense units, dropout, learning rate)  
  - Early stopping to avoid overfitting  

- **Model Training & Evaluation**  
  - Final model training with best hyperparameters  
  - Visualization of accuracy/loss curves  
  - Test-set evaluation with confusion matrix, precision/recall/F1  
  - Sample prediction grid with correct vs. incorrect labeling  

- **Reproducibility**  
  - Fully documented Jupyter notebook with markdown annotations  
  - Saved model in Keras format for easy inference  

---

## 📂 Dataset

**Orvile Brain Cancer MRI Dataset** (Kaggle):  
> https://www.kaggle.com/datasets/orvile/brain-cancer-mri-dataset  

Contains >3,000 T1-weighted contrast-enhanced MRI images across four categories:
- **Glioma**  
- **Meningioma**  
- **Pituitary**  
- **No Tumor**  

---

## 🔧 Getting Started

1. **Clone this repository**  
   ```bash
   git clone https://github.com/sire-magnusss/brain-cancer-cnn-pipeline.git
   cd brain-cancer-cnn-pipeline
