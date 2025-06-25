# Egyptian National ID Classification System – Sahelnaha App

This project is a deep learning solution for classifying Egyptian National ID images using **MobileNetV2**. It was developed as part of a graduation project for the **Sahelnaha** in-home services app.

## 🔍 Overview

The system classifies images as either:
- **ID** (Valid Egyptian National ID card)
- **Not ID**

It supports real-time prediction and is optimized using transfer learning, data augmentation, and evaluation metrics such as ROC curve and confusion matrix.

## 🧠 Model Architecture

- **Base Model**: MobileNetV2 (pre-trained on ImageNet)
- **Layers Added**: GlobalAveragePooling, Dropout, Dense (128), Dense (1 with sigmoid)
- **Loss**: Binary Crossentropy
- **Optimizer**: Adam

## 📁 Project Structure

├── model_training.ipynb # Jupyter Notebook version (if applicable)
├── train_model.py # Training script
├── predict_image.py # Single image prediction script
├── utils/ # Image preprocessing, visualization helpers
├── data/
│ ├── train/
│ ├── val/
│ └── test/
├── mobilenet_id_classifier.h5 # Saved trained model
└── README.md

## 📊 Evaluation

- Accuracy: 95%+
- ROC AUC: ~0.98
- Tools used for evaluation: Confusion matrix, ROC curve

## 🖼️ Sample Prediction

```python
# Run this to classify a single image
python predict_image.py --image_path "path_to_image.jpg"
