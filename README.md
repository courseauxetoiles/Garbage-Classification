# 🗑️ Garbage Classification with CNN Architecture (Without Transfer Learning, and Pre-Trained Model)

A waste sorting system built from scratch with a CNN architecture (no transfer learning, pre-trained model), achieving 87.47% accuracy across 8 categories.

## 📋 Project Overview

This project applies machine learning to practical waste management by:

- Using a custom-designed CNN architecture (without pre-trained models)
- Classifying waste into 8 practical disposal categories
- Optimizing for deployment across multiple platforms

## 📊 Performance

| Metric | Value |
|--------|-------|
| Test Accuracy | 87.47% |
| Test Loss | 0.3816 |

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
```

## 📂 Dataset

Based on the [Kaggle Garbage Classification dataset](https://www.kaggle.com/datasets/mostafaabla/garbage-classification), reorganized into:

- **Organic** - **Recyclable-Paper** - **Recyclable-Plastic** - **Recyclable-Glass**
- **Recyclable-Metal** - **Textile** - **General-Trash** - **Hazardous**

## 🛠️ Implementation

- **Model**: Custom CNN designed from scratch
- **Training**: Data augmentation, stratified splitting, GPU acceleration
- **Output Formats**: SavedModel, TFLite, TFJS

## 📥 Getting Started

Models and dataset available via Google Drive due to file size limitations:

**[Download Data and Models](https://drive.google.com/drive/folders/1iVK8042tgK8rKQYBYIr4s_DhBwuMNIV0?usp=sharing)**

Extract files to their respective directories in the repository structure.

## 📄 License

Available for educational and research purposes.

*Made with Grit by Raihan Ahmad Abiyyu*
