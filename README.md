# 🩺 Skin Lesion Classification using FastAI & PyTorch

<div align="center">

[![Python](https://img.shields.io/badge/Python-3.9%2B-blue?logo=python\&logoColor=white)](https://www.python.org/)
[![FastAI](https://img.shields.io/badge/FastAI-2.7%2B-red?logo=fastai\&logoColor=white)](https://www.fast.ai/)
[![PyTorch](https://img.shields.io/badge/PyTorch-Backend-orange?logo=pytorch\&logoColor=white)](https://pytorch.org/)
[![License](https://img.shields.io/badge/License-MIT-green)](LICENSE)

**A lightweight end-to-end deep learning pipeline for classifying dermatoscopic skin lesion images using transfer learning with FastAI and PyTorch.**

</div>  

---

## 📌 Overview

This project implements a **Convolutional Neural Network (CNN)** with **FastAI** and a **PyTorch backend** to classify skin cancer lesions.
It uses a **ResNet18** model pre-trained on ImageNet and fine-tunes it on dermatoscopic images.

The workflow covers everything from **data collection, preprocessing, augmentation, training, and evaluation** to detailed performance analysis.

> ⚠️ **Disclaimer:** This project is for **educational & research purposes only**. It is *not* a substitute for professional medical diagnosis.

---

## ✨ Key Features

| Feature                             | Description                                                                   |
| :---------------------------------- | :---------------------------------------------------------------------------- |
| 🧠 **Transfer Learning**            | Pre-trained **ResNet18** model fine-tuned with FastAI best practices.         |
| ⚡ **Simplified Workflow**           | FastAI abstracts away boilerplate PyTorch code for faster prototyping.        |
| 🔄 **Data Augmentation**            | Uses `aug_transforms` (flips, rotation, zoom, warp) for generalization.       |
| 📊 **Comprehensive Evaluation**     | Includes **Confusion Matrix**, **Precision-Recall Curve**, and **ROC Curve**. |
| 🎯 **Prediction Demo**              | Load the trained model and run single-image predictions with probabilities.   |
| 🧪 **Test-Time Augmentation (TTA)** | Improves inference robustness by averaging augmented predictions.             |
| 📈 **Learning Rate Finder**         | Automatically selects the best learning rate with `learn.lr_find()`.          |

---

## 📂 Project Structure

```plaintext
Skin-Cancer-Detection-CNN-FastAI/
├── code.ipynb                  # Main Jupyter Notebook
├── dataset.zip                 # Skin cancer dataset
├── literature_review.pdf        # Background research
└── README.md
```

---

## 🧠 Technical Details

* **Model Architecture**: ResNet18
* **Framework**: PyTorch
* **High-Level API**: FastAI
* **Training Strategy**: `fine_tune` + `fit_one_cycle`
* **Metrics**: Accuracy, Precision-Recall, ROC-AUC
* **Visualization**: Confusion Matrix, Top Losses, Optimal LR plots

---

## 🚀 Getting Started

### Prerequisites

* Python 3.9+
* Jupyter Notebook or JupyterLab

### Installation

```bash
# 1. Clone the repository
git clone https://github.com/YOUR_USERNAME/Skin-Cancer-Detection-CNN-FastAI.git
cd Skin-Cancer-Detection-CNN-FastAI

# 2. Install dependencies
pip install fastai timm matplotlib scikit-learn

# 3. Unzip dataset
unzip skincancer1.zip

# 4. Launch Jupyter
jupyter notebook your_notebook_name.ipynb
```

---

## 📊 Results & Visualizations

The model’s performance was assessed using multiple metrics.

<div align="center">  

**Confusion Matrix, Optimal Learning Rate & Top Losses** <img src="https://github.com/user-attachments/assets/9c7e98c9-a187-4cfa-8d82-31499262327d" width="800"/>

**Precision-Recall & ROC Curves** <img src="https://github.com/user-attachments/assets/5dd71f0c-37b6-4c93-8f15-9aec7129a3a9" width="800"/>

</div>  

---

## 📄 License

This project is licensed under the **MIT License**. See the [LICENSE](LICENSE) file for details.

---

## 👨‍💻 Author

<div align="center">

**[A. Jayavanth](https://github.com/jayavanth18)**

[![GitHub](https://img.shields.io/badge/GitHub-jayavanth18-black?logo=github)](https://github.com/jayavanth18)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-Connect-blue?logo=linkedin)](https://www.linkedin.com/in/jayavanth18/)

⭐ If this repo helped you, please consider giving it a **star**!

</div>  

---
