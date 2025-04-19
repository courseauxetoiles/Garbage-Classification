# 🗑️ Garbage Classification with Custom CNN (No Transfer Learning)

This project focuses on classifying various types of garbage into refined categories using a custom-built Convolutional Neural Network (CNN), without relying on transfer learning. The goal is to enable practical waste sorting based on how each type of waste should be processed or disposed.

## 📂 Dataset Overview

* **Source:** Garbage Classification Dataset - Kaggle
* **Original Classes:** 12 (battery, biological, brown-glass, etc.)
* **Reorganized Classes:** Grouped into 8 categories based on real-world waste management principles:
   * **Organic**
   * **Recyclable-Paper**
   * **Recyclable-Plastic**
   * **Recyclable-Glass**
   * **Recyclable-Metal**
   * **Textile**
   * **General-Trash**
   * **Hazardous**

## 📊 Model Performance

* **Test Accuracy:** 87.47%
* **Test Loss:** 0.3816

### Classification Report:
```
                    precision    recall  f1-score   support

     general-trash       0.85      0.69      0.76       105
         hazardous       0.91      0.73      0.81       142
           organic       0.93      0.85      0.89       148
  recyclable-glass       0.84      0.85      0.85       302
  recyclable-metal       0.72      0.69      0.70       116
  recyclable-paper       0.90      0.82      0.86       292
recyclable-plastic       0.76      0.73      0.75       130
           textile       0.90      0.97      0.93      1096

          accuracy                           0.87      2331
         macro avg       0.85      0.79      0.82      2331
      weighted avg       0.87      0.87      0.87      2331
```

## 🔧 What This Project Does

* Explores and re-categorizes garbage classes for better alignment with disposal methods.
* Applies data augmentation for minority classes and stratified splitting.
* Trains a CNN model from scratch using TensorFlow on Google Colab with GPU support.
* Visualizes the training process (accuracy/loss curves).
* Converts the trained model into formats suitable for deployment:
   * `SavedModel` (TensorFlow)
   * `TFLite` (for mobile/embedded)
   * `TFJS` (for web applications)

## 🚀 Deployment-Ready Outputs

* `SavedModel` for server/cloud-based inference
* `TFLite` for Android or microcontrollers
* `TFJS` for in-browser JavaScript applications

## 📥 Get the Data and Models

Due to file size limitations on GitHub, the data and model files are stored separately. You can download them from Google Drive:

**[Download Data and Models](https://drive.google.com/drive/folders/1iVK8042tgK8rKQYBYIr4s_DhBwuMNIV0?usp=sharing)**

After downloading, place the files in their corresponding directories in your local repository:
- Place dataset files in the `data` folder
- Place models in their respective folders:
  - `saved_model` for TensorFlow SavedModel
  - `tflite` for TensorFlow Lite model
  - `tfjs_model` for TensorFlow.js model

## 🛠️ How to Use

1. Clone this repository
2. Download the data and models from the Google Drive link above
3. Extract the files to their appropriate directories
4. Run the notebook `garbage_classification_cnn.ipynb` to train the model or use the pre-trained models for inference

Feel free to use this model for educational, research, or prototyping purposes!

*Made with grit and GPU by Raihan Ahmad Abiyyu*
