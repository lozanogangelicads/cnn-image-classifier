# 🧠 Convolutional Neural Network for Image Classification

## 📘 Course Assignment  
**Applied Machine Learning**  
Author: Angelica Lozano  

---

## 📌 Overview  
This project demonstrates how to build and train a **Convolutional Neural Network (CNN)** to classify images into one of 10 categories. It includes both a base CNN and a transfer learning model that builds upon the features learned by the original network.

Two models were developed:
- A custom CNN trained from scratch
- A shallow classifier built on top of the frozen CNN (transfer learning)

---

## 🧪 Methodology

### 🔹 Step 1: Model Development
- Used a CIFAR-10-like dataset (10 classes)
- Applied normalization and one-hot encoding
- Built a custom CNN architecture:
  - Conv2D → MaxPooling → Dropout (repeated)
  - Flatten + Dense layers

### 🔹 Step 2: Transfer Learning Classifier
- Extracted embeddings from frozen base CNN
- Built new classifier using fully connected layers
- Reduced overfitting with dropout
- Saved final model as `classification_model_.h5`

---

## 📈 Key Results

- The base CNN and transfer learning classifier both achieved high accuracy
- Transfer learning provided faster training and improved generalization
- Models are ready for deployment or further experimentation

---

## 📁 Project Files
cnn-image-classifier/
- Convolutional Neural Networks.ipynb # Jupyter Notebook with full pipeline
- CNN_model_.h5 # Saved base CNN model
- classification_model_.h5 # Final transfer learning model
- README.md # This documentation file

### 4. 🧠 [CNN Image Classification (CIFAR-10)](https://github.com/lozanogangelicads/cnn-image-classifier)
- Built custom CNN and transfer learning model for image classification.
- Tools: TensorFlow, Keras, NumPy, Matplotlib
