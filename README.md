# 👗 Fashion MNIST Classification using ANN  
## 🔬 Weight Initializer Comparison (Glorot vs He Normal vs LeCun)

This project implements an Artificial Neural Network (ANN) to classify Fashion MNIST images and compares three different weight initialization techniques: Glorot Uniform, He Normal, and LeCun Normal.

The goal is to analyze how different initializers impact model performance, convergence, and accuracy.

---

## 📌 Project Overview

In deep learning, weight initialization plays a critical role in:

- Model convergence speed  
- Training stability  
- Final accuracy  
- Overfitting behavior  

This project evaluates and visualizes the performance of three popular initialization methods using the same ANN architecture.

---

## 📂 Dataset

Fashion MNIST Dataset:
- 60,000 training images
- 10,000 test images
- 10 classes (clothing categories)
- 28x28 grayscale images

Classes include:
T-shirt, Trouser, Pullover, Dress, Coat, Sandal, Shirt, Sneaker, Bag, Ankle Boot

---

## 🧠 Model Architecture (ANN Only – No CNN)

- Input Layer: Flatten (28x28)
- Hidden Layer 1: Dense (256 neurons, ReLU)
- Hidden Layer 2: Dense (128 neurons, ReLU)
- Output Layer: Dense (10 neurons, Softmax)

Optimizer: Adam  
Loss Function: Sparse Categorical Crossentropy  
Epochs: 20  
Batch Size: 128  

---

## ⚙ Initializers Compared

- Glorot Uniform (Xavier Initialization)
- He Normal Initialization
- LeCun Normal Initialization

Each model is trained using the same architecture and hyperparameters for fair comparison.

---

## 📊 Evaluation Metrics

The models are evaluated using:

- Test Accuracy
- Test Loss
- Confusion Matrix
- Heatmap Visualization
- Accuracy Comparison Bar Chart
- Loss Comparison Bar Chart
- Train vs Validation Accuracy Comparison

---

## 📈 Key Observations

- He Normal generally performs better with ReLU activation.
- Glorot provides stable and balanced performance.
- LeCun works best with SELU activation but is tested here with ReLU for comparison.

(Results may vary slightly depending on training run.)

---

## 💾 Saved Models

The trained models are saved in `.keras` format:

- glorot_model.keras
- he_normal_model.keras
- lecun_model.keras

---

## 🚀 How to Run

1. Install dependencies:
   pip install tensorflow numpy matplotlib scikit-learn

2. Run the Python script:
   python filename.py

---

## 🛠 Technologies Used

- Python
- TensorFlow / Keras
- NumPy
- Matplotlib
- Scikit-learn

---

## 🎯 Learning Outcomes

- Understanding ANN implementation
- Comparing weight initialization techniques
- Visualizing confusion matrices and performance metrics
- Analyzing train vs validation performance
- Practical deep learning experimentation


