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

This project implements a **Convolutional Neural Network (CNN)** using **FastAI** and a **PyTorch backend** to classify skin cancer lesions from dermatoscopic images.

It uses a **ResNet18** model pre-trained on ImageNet and fine-tunes it on a curated subset of the **Skin Cancer ISIC** dataset.

> ⚠️ **Disclaimer:** This project is for **educational & research purposes only**. It is *not* a substitute for professional medical diagnosis.

> ⚠️ **Note:** Due to resource and training time constraints, the notebook uses only a **subset of classes** (some classes were removed) from the original dataset.


---
## ✨ Key Features

| Feature | Description |
| :--- | :--- |
| 🧠 **Transfer Learning** | Pre-trained **ResNet18** model fine-tuned with FastAI best practices. |
| ⚡ **Simplified Workflow** | FastAI abstracts away boilerplate PyTorch code for faster prototyping. |
| 🔄 **Data Augmentation** | Uses `aug_transforms` (flips, rotation, zoom, warp) for generalization. |
| 📊 **Comprehensive Evaluation** | Includes **Confusion Matrix**, **Precision-Recall Curve**, and **ROC Curve**. |
| 🎯 **Prediction Demo** | Load the trained model and run single-image predictions with probabilities. |
| 🧪 **Test-Time Augmentation (TTA)** | **Achieved 80.68% accuracy** by averaging predictions over augmented images. |
| 📈 **Learning Rate Finder** | Automatically selects the best learning rate with `learn.lr_find()`. |

---

## 📂 Project Structure

```plaintext
Skin-Cancer-Detection-CNN-FastAI/
├── code.ipynb                  # Main Jupyter Notebook
├── README.md                   # Project documentation
├── literature_review.pdf       # Background research
```

---

## 📦 Dataset

We use the publicly available **Skin Cancer ISIC** dataset from Kaggle:
🔗 [Skin Cancer 9 Classes (ISIC) - Kaggle](https://www.kaggle.com/datasets/nodoubttome/skin-cancer9-classesisic)

**Important Note:**
To reduce training time and manage resources, the notebook does **not use all 9 classes**. One or more classes were **intentionally excluded** during training. You can modify the notebook to include all classes if needed.

---

## 🧠 Technical Details

* **Model Architecture**: ResNet18
* **Framework**: PyTorch
* **High-Level API**: FastAI
* **Training Strategy**: `fine_tune` + `fit_one_cycle`
* **Metrics**: Accuracy, Precision-Recall, ROC-AUC
* **Visualization**: Confusion Matrix, Top Losses, Optimal LR plots
* **Dataset Subsetting**: Some classes from the original ISIC dataset were excluded for practical training duration.

---

## 🚀 Getting Started

### Prerequisites

* Python 3.9+
* Jupyter Notebook or JupyterLab
* Kaggle API (for downloading dataset if not manually done)

### Installation

```bash
# 1. Clone the repository
git clone https://github.com/YOUR_USERNAME/Skin-Cancer-Detection-CNN-FastAI.git
cd Skin-Cancer-Detection-CNN-FastAI

# 2. Install dependencies
pip install fastai timm matplotlib scikit-learn

# 3. Download dataset (manually or via Kaggle CLI)
# Example using Kaggle CLI:
kaggle datasets download -d nodoubttome/skin-cancer9-classesisic
unzip skin-cancer9-classesisic.zip

# 4. Launch Jupyter
jupyter notebook code.ipynb
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

## 👨‍💻 Authors

<div align="center">

### 🔹 [A. Jayavanth](https://github.com/jayavanth18)

[![GitHub](https://img.shields.io/badge/GitHub-jayavanth18-181717?style=for-the-badge\&logo=github)](https://github.com/jayavanth18)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-jayavanth18-0A66C2?style=for-the-badge\&logo=linkedin)](https://www.linkedin.com/in/jayavanth18/)

---

### 🔹 [Surya](https://github.com/surya2508)

[![GitHub](https://img.shields.io/badge/GitHub-surya2508-181717?style=for-the-badge\&logo=github)](https://github.com/surya2508)

---

### 🔹 [Nayana](https://github.com/nayana-3110)

[![GitHub](https://img.shields.io/badge/GitHub-nayana--3110-181717?style=for-the-badge\&logo=github)](https://github.com/nayana-3110)

---

⭐️ If you found this repository helpful, please consider giving it a **star**!

</div>
