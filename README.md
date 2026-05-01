# 🧠 Medical Image Classification using DenseNet-121

A deep learning project that classifies medical images into **binary classes (YES/NO)** using a fine-tuned DenseNet-121 model with explainability via Grad-CAM.

---

## 🚀 Project Overview

This project focuses on building a robust medical image classifier capable of detecting the presence (YES) or absence (NO) of a condition from images.

Key highlights:
- Transfer learning with DenseNet-121
- Custom classifier head
- Data augmentation & regularization
- Evaluation using precision, recall, F1-score
- Grad-CAM visualization for explainability

---

## 🧠 Model Architecture

- Backbone: DenseNet-121 (pretrained on ImageNet)
- Custom classifier:
  - Linear → ReLU → Dropout → Linear
- Fine-tuning:
  - Frozen backbone + partially unfrozen final dense blocks

---

## 📊 Results

| Metric | Score |
|-------|------|
| Accuracy | **92%** |
| Precision | 0.94 |
| Recall | 0.94 |
| F1-score | 0.94 |

### Confusion Matrix


[[18 2]
[ 2 29]]


---

## 🔍 Explainability (Grad-CAM)

Grad-CAM is used to visualize model attention:

- Highlights regions influencing predictions
- Helps validate model behavior
- Critical for medical AI trust

---

## 🛠️ Tech Stack

- Python
- PyTorch
- Torchvision
- OpenCV
- Matplotlib
- Scikit-learn

---

## ⚙️ Installation

```bash
git clone https://github.com/Nis03-ui/Brain-tumor-detection-through-MRI-Scan
cd medical-image-classifier
