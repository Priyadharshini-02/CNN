#  Image Classification Using CNN (CIFAR-10)

## Overview  
This project implements a **Convolutional Neural Network (CNN)** using TensorFlow/Keras to classify **CIFAR-10 images** into 10 categories (airplane, cat, ship, etc.).  
The notebook also supports **predicting new images** from local files or Google Drive.

---

## Model  
- Convolutional + Pooling + Dropout layers  
- Fully connected layers with **ReLU** and **Softmax**  
- Trained with **Adam optimizer** and **categorical cross-entropy**

---

## Results  
- Accuracy: ~75–85% (varies by hyperparameters)  
- CNN outperforms MLP due to spatial feature extraction  
- Hardest classes: *cat vs dog*, *deer vs horse*

---

## Predict New Image  
```python
predict_new_image(model, 
  "https://drive.google.com/file/d/1MBEAeE0YGL5bop_NxejONVAaC52kXsP7/view?usp=sharing", 
  from_drive=True)
```
Supports: Local files, URLs, or Google Drive links.

---

## Requirements  
```bash
pip install tensorflow numpy matplotlib pillow requests
```

---

## 🚀 Run  
1. Open **ImageClassificationUsingCNN.ipynb** in Colab/Jupyter  
2. Run all cells to train and evaluate  
3. Use `predict_new_image()` to test on custom images  
