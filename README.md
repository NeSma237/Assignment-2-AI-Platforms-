# 🧠 Fashion-MNIST Classification using PyTorch

## 📌 Overview  
This project implements a **Multilayer Perceptron (MLP)** using **PyTorch** to classify images from the **Fashion-MNIST** dataset.  
The model is trained on grayscale clothing images (28×28) and learns to predict one of ten fashion categories such as *T-shirt, Dress, Sneaker,* etc.  

---

## ⚙️ File  
**`Assignment_2_Fashion-MNIST(AI Platforms).ipynb`**  
Contains all code for:  
- Data loading and preprocessing  
- Model definition and training  
- Evaluation and visualization (confusion matrix, accuracy plots, and predictions)

---

## 🧩 Model Architecture  
| Layer | Type | Input → Output | Activation |
|:------|:------|:----------------|:------------|
| 1 | Linear | 784 → 256 | ReLU |
| 2 | Linear | 256 → 128 | ReLU |
| 3 | Linear | 128 → 10 | — |

**Loss Function:** CrossEntropyLoss  
**Optimizer:** Adam (lr = 0.001)  
**Epochs:** 9  
**Batch Size:** 64  

---

## 📊 Results  
- **Training Accuracy:** 0.916  
- **Test Accuracy:** 0.885  

✅ The model shows strong generalization with smooth convergence and consistent accuracy improvement.  
🧩 The confusion matrix highlights common misclassifications between similar clothing items (e.g., Shirt vs T-shirt).  

---

## 📈 Visualizations  
- Confusion matrix (color-coded per class)  
- 4×4 grid of test images with predicted & true labels (green = correct, red = incorrect)  
- Training loss and accuracy curves per epoch  

---

## 💡 Possible Improvements  
- Add normalization to input images  
- Use dropout for regularization  
- Increase epochs for higher accuracy  
- Try CNN architectures for improved performance  

---

## 📝 Requirements  
```
torch
torchvision
matplotlib
scikit-learn
```

Install via pip:  
```bash
pip install torch torchvision matplotlib scikit-learn
```

---

## 📬 Author  
**Nesma Nasser**  
Project submitted for **AI Platforms — Assignment 2**  
