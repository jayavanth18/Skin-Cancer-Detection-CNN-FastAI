# 🩺 Skin Cancer Detection with Deep Learning

<div align="center">

![Python](https://img.shields.io/badge/Python-3.x-blue.svg)
![FastAI](https://img.shields.io/badge/FastAI-2.x-red.svg)
![License](https://img.shields.io/badge/License-MIT-green.svg)

**A deep learning pipeline for classifying skin cancer lesions using FastAI and ResNet18, with full evaluation metrics and visualizations.**

</div>  

---

## 📌 Overview

This project implements a **Convolutional Neural Network (CNN)** using the **FastAI library** to classify different types of **skin cancer lesions**.
It leverages **ResNet18** (pre-trained on ImageNet) and fine-tunes it on the provided dataset.

The workflow includes:

* Data preprocessing and augmentation
* Model training & fine-tuning
* Confusion Matrix & Learning Rate Finder
* Precision-Recall and ROC Curves
* Test-time prediction with probability visualization

---

## ✨ Features

* 📂 **Custom Dataset** – ZIP file with labeled images of skin lesions
* 🔄 **Data Augmentation** – Improves generalization using FastAI `aug_transforms`
* 🧠 **Transfer Learning** – ResNet18 backbone fine-tuned on dataset
* 📊 **Evaluation Metrics** – Confusion matrix, Precision-Recall, ROC curves
* 🎯 **Prediction Demo** – Classify test images with probabilities

---

## 📂 Project Structure

```plaintext
Skin-Cancer-Detection-CNN-FastAI/
├── code.ipynb                  # Main Jupyter Notebook
├── dataset.zip                 # Skin cancer dataset
├── literature_review.pdf        # Background research
├── results/
│   ├── confusion_matrix.png
│   ├── optimal_lr.png
│   ├── predictions.png
│   ├── pr_curve.png
│   └── roc_curve.png
└── README.md
```

---

## ⚙️ Installation

1. Clone this repository:

```bash
git clone https://github.com/YOUR_USERNAME/Skin-Cancer-Detection-CNN-FastAI.git
cd Skin-Cancer-Detection-CNN-FastAI
```

2. Install dependencies:

```bash
pip install fastai timm matplotlib scikit-learn
```

---

## 🚀 Usage

1. Extract the dataset:

```bash
unzip dataset.zip
```

2. Open and run the notebook:

```bash
jupyter notebook code.ipynb
```

3. Train the model (default: ResNet18, 25 epochs fine-tuning).

---

## 📊 Results

### 🔹 Confusion Matrix, Optimal Learning Rate & Predictions 

<img width="1040" height="300" alt="Confusion Matrix, Optimal LR, Predictions" src="https://github.com/user-attachments/assets/9c7e98c9-a187-4cfa-8d82-31499262327d" />


### 🔹 Precision-Recall Curve & ROC Curve
<img width="973" height="400" alt="PR Curve, ROC Curve" src="https://github.com/user-attachments/assets/5dd71f0c-37b6-4c93-8f15-9aec7129a3a9" />



---

## 🧪 Example Prediction

```python
img = PILImage.create("Test/vascular lesion/ISIC_0024370.jpg")
pred_class, pred_idx, pred_probs = learn.predict(img)

print(f"Predicted Class: {pred_class}")
print(f"Probabilities: {pred_probs}")
```

✅ Output Example:

```
Predicted Class: vascular lesion  
Predicted Probabilities: [0.01, 0.03, 0.92, 0.04]
```

---

## 📄 License

This project is licensed under the **MIT License** – see [LICENSE](LICENSE) for details.

---

## 👨‍💻 Author

<div align="center">

**[A. Jayavanth](https://github.com/jayavanth18)**

[![GitHub](https://img.shields.io/badge/GitHub-jayavanth18-black?logo=github)](https://github.com/jayavanth18)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-Connect-blue?logo=linkedin)](https://www.linkedin.com/in/jayavanth18/)

⭐ If this repo helped you, please consider giving it a **star**!

</div>  

---

Do you also want me to write a **one-line tagline for GitHub repo (the short description that shows under repo name)**, optimized for recruiters/professors?
