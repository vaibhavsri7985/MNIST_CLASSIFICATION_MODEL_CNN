# 🧠 CNN Image Classification Projects (Fashion MNIST & MNIST)

## 📌 Project Overview
This repository contains two deep learning projects that use **Convolutional Neural Networks (CNNs)** for image classification:  

1. **Fashion MNIST Classification** – Automatically classifies clothing items into 10 categories.  
2. **MNIST Digit Classification** – Recognizes handwritten digits (0–9).  

These projects showcase how CNNs can effectively learn image features such as edges, textures, and shapes, and apply them for accurate predictions.  

---

## 📊 Datasets

### 🔹 Fashion MNIST
- **Images**: 70,000 grayscale images of fashion products.  
- **Resolution**: 28x28 pixels.  
- **Classes** (10 categories):  
  - T-shirt/top  
  - Trouser  
  - Pullover  
  - Dress  
  - Coat  
  - Sandal  
  - Shirt  
  - Sneaker  
  - Bag  
  - Ankle boot  

### 🔹 MNIST (Handwritten Digits)
- **Images**: 70,000 grayscale images of handwritten digits.  
- **Resolution**: 28x28 pixels.  
- **Classes**: Digits from 0 to 9.  

Both datasets are well-known benchmarks for evaluating deep learning models in image recognition.

---

## ⚙️ Methodology

### 1. Data Preprocessing
- Normalized pixel values (0–255 → 0–1).  
- Reshaped images to fit CNN input (28x28x1).  
- Converted labels into categorical format (one-hot encoding).  

### 2. Model Architecture (CNN)
- **Convolutional layers**: Extract spatial features (edges, textures).  
- **MaxPooling layers**: Downsample feature maps to reduce complexity.  
- **Dropout layers**: Reduce overfitting.  
- **Fully connected dense layers**: Perform classification.  
- **Softmax output**: Predicts probabilities across 10 classes.  

### 3. Training Strategy
- Optimizer: **Adam**.  
- Loss function: **Categorical Crossentropy**.  
- Metrics: **Accuracy**.  
- Callbacks:  
  - **EarlyStopping** → Stops training when validation loss stops improving.  
  - **ReduceLROnPlateau** → Dynamically reduces learning rate when model plateaus.  

### 4. Evaluation
- Compared **training vs validation loss/accuracy**.  
- Ensured minimal overfitting.  
- Evaluated on test datasets.  

---

## 📈 Results

### 🔹 Fashion MNIST
- **Training Accuracy**: ~92%  
- **Testing Accuracy**: ~90%  
- Observation: Slight gap between training and testing accuracy, but still good generalization.  

### 🔹 MNIST (Handwritten Digits)
- **Training Accuracy**: 95%+  
- **Testing Accuracy**: 95%+  
- Observation: Model performed excellently, with minimal gap between training and test performance.  

---

