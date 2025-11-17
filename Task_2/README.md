# ✍️ Handwritten Character Recognition (MNIST)


## 🚀 Project Overview  
- This project focuses on building a **Convolutional Neural Network (CNN)** for recognizing handwritten **digits (0–9)** using the **MNIST dataset**.

---

## 🎯 Objectives  
- Identify handwritten digits and characters  
- Apply core image preprocessing techniques  
- Train a CNN from scratch  
- Test the model on custom handwritten inputs  
- Visualize accuracy, loss, and the confusion matrix   

---

## 🧰 Key Features  
- Dataset: **MNIST** for digits (0–9)   
- Model: **Convolutional Neural Network (CNN)** built using Keras  
- Image preprocessing pipeline for new user-uploaded images  
- Evaluation using:
  - Accuracy  
  - Loss  
  - Confusion Matrix  

---

## 📂 Dataset Information  

### **MNIST Dataset (Used in Current Code)**
- 70,000 handwritten digit images  
- 60,000 train, 10,000 test  
- Image size: **28×28**, grayscale  

Loaded via:

```python
from keras.datasets import mnist
(X_train, y_train), (X_test, y_test) = mnist.load_data()
```
---
## ⚙️ Tech Stack
- Python
- Keras
- Sklearn
- Numpy
- Matplotlib
---
## 👩🏻‍💻Author
```Debaswini-M```
