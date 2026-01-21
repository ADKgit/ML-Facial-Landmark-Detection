# Facial Landmark Prediction Using Machine Learning

This repository contains the implementation of a **facial landmark alignment system** developed as part of an **Applied Machine Learning coursework**.  
The project focuses on predicting key facial landmark points from images using **classical computer vision techniques** combined with **supervised machine learning regression models**.

---

## 📌 Project Overview

Facial landmark alignment is a fundamental problem in computer vision, with applications in face recognition, emotion analysis, and human–computer interaction.  
In this project, a full end-to-end pipeline was implemented to:

- Load and preprocess facial image datasets
- Extract meaningful visual features from images
- Train regression models to predict facial landmark coordinates
- Evaluate prediction accuracy using quantitative error metrics
- Visualise predicted landmarks against ground-truth annotations

The emphasis is on **understanding and implementing the full machine learning pipeline**, rather than relying on pre-built face alignment libraries.

---

## 🧠 Methodology

The pipeline follows these key stages:

1. **Data Loading & Preprocessing**
   - Facial images and corresponding landmark annotations are loaded
   - Images are normalised and resized for consistency
   - Landmark coordinates are scaled appropriately

2. **Feature Extraction**
   - Local image descriptors are extracted from facial regions
   - These descriptors provide robust representations of facial structure

3. **Regression Model Training**
   - A supervised regression model is trained to map image features to landmark coordinates
   - The model learns spatial relationships between facial features

4. **Prediction & Evaluation**
   - The trained model predicts landmark positions on unseen test images
   - Performance is measured using **Euclidean distance error** between predicted and true landmarks

5. **Visualisation**
   - Predicted landmarks are overlaid on facial images
   - Qualitative inspection complements quantitative evaluation

---

## 📊 Evaluation

Model performance is evaluated using:
- **Mean Euclidean distance error** across facial landmarks
- Visual comparison between predicted and ground-truth landmark positions

This allows both numerical and visual assessment of alignment quality.

---

## 🛠 Technologies Used

- **Python**
- **NumPy**
- **scikit-learn**
- **OpenCV**
- **Matplotlib**
- **Jupyter Notebook**

---

## 📁 Repository Structure

```text
.
├── Task 2.ipynb        # Main notebook containing full pipeline
├── data/              # Facial images and landmark annotations
├── results/           # Prediction outputs and evaluation results
└── README.md          # Project documentation
