# 🗑️ Garbage Classification with Custom CNN (No Transfer Learning)

This project focuses on classifying various types of garbage into meaningful categories using a custom-built Convolutional Neural Network (CNN), without relying on transfer learning. The goal is to enable practical waste sorting based on how each type of waste should be processed or disposed.

## 📂 Dataset Overview

- **Source:** [Garbage Classification Dataset - Kaggle](https://www.kaggle.com/datasets/mostafaabla/garbage-classification)
- **Original Classes:** 12 (battery, biological, brown-glass, etc.)
- **Reorganized Classes:** Grouped into 6 categories based on real-world waste management principles:
  - **Organic**
  - **Recyclable**
  - **Residual**
  - **Hazardous**
  - **Textile**
  - **Glass**

## 🔧 What This Project Does

- Explores and re-categorizes garbage classes for better alignment with disposal methods.
- Applies data augmentation for minority classes and stratified splitting.
- Trains a CNN model from scratch using TensorFlow on Google Colab with GPU support.
- Visualizes the training process (accuracy/loss curves).
- Converts the trained model into formats suitable for deployment:
  - `SavedModel` (TensorFlow)
  - `TFLite` (for mobile/embedded)
  - `TFJS` (for web applications)

## 🚀 Deployment-Ready Outputs

- `SavedModel` for server/cloud-based inference
- `TFLite` for Android or microcontrollers
- `TFJS` for in-browser JavaScript applications

---

Feel free to use this model for educational, research, or prototyping purposes!

> *Made with grit and GPU by Raihan Ahmad Abiyyu*
