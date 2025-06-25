# Egyptian National ID Classification System – Sahelnaha App

This project uses a deep learning model based on MobileNetV2 to classify images as Egyptian National ID or not. Developed as part of a graduation project for the Sahelnaha in-home services app.

## 📄 File
- `final_ids.ipynb`: Jupyter Notebook containing full model training, evaluation (ROC, confusion matrix), and prediction code.

## 🧠 Features
- Transfer learning with MobileNetV2
- Data augmentation and fine-tuning
- Evaluation using AUC, ROC, and confusion matrix
- Real-time prediction on new images

## 🛠️ Tech Stack
Python, TensorFlow, Keras, OpenCV, Matplotlib, Seaborn

## ▶️ How to Run
1. Install dependencies:
pip install tensorflow opencv-python matplotlib seaborn scikit-learn

2. Open the notebook:
jupyter notebook final_ids.ipynb


3. Run all cells.

## 📦 Output
- Trained model: `mobilenet_id_classifier.h5`

