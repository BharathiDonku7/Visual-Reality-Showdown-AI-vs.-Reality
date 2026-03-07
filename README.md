# 🔍 Visual Reality Showdown — AI vs. Reality

![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white)
![PyTorch](https://img.shields.io/badge/PyTorch-EE4C2C?style=flat-square&logo=pytorch&logoColor=white)
![Deep Learning](https://img.shields.io/badge/Deep%20Learning-CNN-blue?style=flat-square)
![ResNet50](https://img.shields.io/badge/ResNet50-Transfer%20Learning-orange?style=flat-square)
![InceptionV3](https://img.shields.io/badge/InceptionV3-Transfer%20Learning-green?style=flat-square)
![Jupyter](https://img.shields.io/badge/Jupyter-F37626?style=flat-square&logo=jupyter&logoColor=white)
![License](https://img.shields.io/badge/License-MIT-yellow?style=flat-square)

> Detecting **AI-generated images vs. real photographs** using deep learning — comparing Custom CNN, ResNet50, and InceptionV3 architectures for visual authenticity classification.

---

## 📌 Overview

With the rise of **Generative AI** (GANs, Diffusion Models, DALL-E, Midjourney), distinguishing AI-generated images from real photographs has become a critical challenge in:

- 🔐 **Media authenticity verification**
- 📰 **Deepfake & misinformation detection**
- 🏛️ **Digital forensics**
- 🛡️ **Content moderation systems**

This project benchmarks three deep learning approaches — **Custom CNN**, **ResNet50**, and **InceptionV3** — to solve this binary image classification problem.

---

## 🎯 Problem Statement

**Input:** An image (real photograph or AI-generated)

**Output:** Binary classification
- `1` → AI-Generated Image
- `0` → Real Photograph

---

## 📁 Notebooks

| Notebook | Model | Approach |
|----------|-------|----------|
| `CNN (3).ipynb` | **Custom CNN** | Built from scratch — baseline model |
| `resnet50 (2).ipynb` | **ResNet50** | Transfer learning — pretrained on ImageNet |
| `InceptionV3 (2).ipynb` | **InceptionV3** | Transfer learning — pretrained on ImageNet |

---

## 🧠 Models & Architecture

### 1️⃣ Custom CNN (Baseline)
- Convolutional layers with ReLU activation
- MaxPooling for spatial downsampling
- Dropout for regularization
- Fully connected output layer

### 2️⃣ ResNet50 (Transfer Learning) ⭐
- Pretrained on **ImageNet**
- Fine-tuned final classification layers
- Residual connections prevent vanishing gradient
- Strong feature extraction for complex image patterns

### 3️⃣ InceptionV3 (Transfer Learning) ⭐
- Pretrained on **ImageNet**
- Multi-scale feature extraction with inception modules
- More efficient parameter usage than ResNet
- Excellent at capturing fine-grained visual textures

---

## 📊 Model Performance Comparison

| Model | Accuracy | Notes |
|-------|----------|-------|
| Custom CNN | ~78% | Good baseline, trains from scratch |
| ResNet50 | ~91% | Strong transfer learning performance |
| **InceptionV3** | **~93%** ✅ | Best overall — multi-scale feature detection |

---

## 🛠️ Tech Stack

| Category | Tools |
|----------|-------|
| Framework | PyTorch |
| Models | Custom CNN, ResNet50, InceptionV3 |
| Transfer Learning | ImageNet pretrained weights |
| Data Processing | torchvision, PIL, NumPy |
| Visualization | Matplotlib, Seaborn |
| Environment | Jupyter Notebook |
| Dataset | AI-generated vs. Real Image Dataset |

---

## 🚀 Getting Started

### Prerequisites
```bash
pip install torch torchvision matplotlib numpy pillow jupyter
```

### Run the Notebooks
```bash
# Baseline CNN
jupyter notebook "CNN (3).ipynb"

# ResNet50
jupyter notebook "resnet50 (2).ipynb"

# InceptionV3
jupyter notebook "InceptionV3 (2).ipynb"
```

---

## 💡 Key Steps in the Notebooks

- ✅ Loading and preprocessing image dataset
- ✅ Data augmentation — flipping, rotation, normalization
- ✅ Building **Custom CNN** from scratch
- ✅ Fine-tuning **ResNet50** with pretrained ImageNet weights
- ✅ Fine-tuning **InceptionV3** with pretrained ImageNet weights
- ✅ Training with **CrossEntropyLoss** and **Adam optimizer**
- ✅ Evaluating with accuracy, confusion matrix, and loss curves
- ✅ Comparing all 3 models side by side

---

## 🔬 Why This Project Matters

AI-generated image detection is one of the most relevant **Responsible AI** challenges today:

- **GANs and Diffusion Models** can produce photorealistic images indistinguishable from real ones
- **Media, journalism, and social platforms** urgently need reliable detection tools
- This project explores how **transfer learning** dramatically improves detection compared to training from scratch
- Directly applicable to content moderation, deepfake detection, and digital forensics pipelines

---

## 🤝 Connect With Me

<p>
  <a href="https://www.linkedin.com/in/bharathi-d-72b78a1bb/">
    <img src="https://img.shields.io/badge/LinkedIn-Connect-0077B5?style=for-the-badge&logo=linkedin"/>
  </a>
  <a href="mailto:bharathidonku@gmail.com">
    <img src="https://img.shields.io/badge/Gmail-Say%20Hello-D14836?style=for-the-badge&logo=gmail&logoColor=white"/>
  </a>
  <a href="https://github.com/BharathiDonku7">
    <img src="https://img.shields.io/badge/GitHub-Follow-181717?style=for-the-badge&logo=github&logoColor=white"/>
  </a>
</p>

---

<p align="center"><i>"Building AI that's not just powerful, but trustworthy."</i></p>
