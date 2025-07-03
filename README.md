# ♻️ Recyclable Classifier – TensorFlow Lite + MobileNetV2

A lightweight, real-time image classification model designed to detect 7 recyclable material classes using TensorFlow Lite. Trained on a dataset of 63,000 images and optimized for deployment on edge devices.

---

## 📦 Project Overview

As part of the Power Learn Project AI for Software Engineering module, this project aims to promote sustainable technology by enabling automated identification of recyclable materials using machine learning.

---

## 🚀 Features

- ✅ Transfer learning with MobileNetV2 pretrained on ImageNet
- ✅ 63,000+ images across 7 recyclable categories
- ✅ `.tflite` model export for mobile deployment
- ✅ Clean GitHub structure with reproducible Jupyter workflow
- ✅ Performance visualization with `matplotlib`

---

## 📁 Repository Structure

recyclable-classifier/ │ ├── recyclable_classifier.ipynb # Jupyter Notebook (training, inference) ├── recycle_model.tflite # Exported TensorFlow Lite model ├── recycle_model/ # SavedModel directory ├── images/ # Sample input/output image examples ├── utils/ # Preprocessing scripts (optional) ├── README.md # Project documentation (this file) └── requirements.txt # Required packages (for pip install)


---

## 🧠 Model Architecture

- Base: `MobileNetV2` (frozen layers)
- Custom head:
  - `GlobalAveragePooling2D`
  - `Dense (softmax)` – 7 output classes
- Loss: `SparseCategoricalCrossentropy`
- Optimizer: `Adam`

---

## 📊 Dataset

- **Classes**: Plastic, Paper, Metal, Glass, Cardboard, Trash, Compost
- **Total Samples**: 63,000
- **Split**:
  - Training: 50,400
  - Validation: 12,600
- **Preprocessing**:
  - Resized to `(224, 224)`
  - Normalized to [0, 1] pixel values
  - Augmented via shuffle + batching

---

## 💡 Getting Started

### 1. Clone the repository

```bash
git clone https://github.com/leonard-dev/recyclable-classifier.git
cd recyclable-classifier

### 3. Install Dependencies

Activate your virtual environment, then run:

```bash
pip install -r requirements.txt


Want me to drop that into the GitHub README automatically for you, fully formatted?

---

### 🧪 Bonus: Freeze a Clean Environment (Optional)

Later, when you're ready to finalize submission:
- Double-check only the necessary packages are in the `.txt` (i.e., remove dev or redundant packages)
- You can edit it manually to include only things like: `tensorflow`, `matplotlib`, `numpy`, etc.

---

Say the word if you'd like help tidying the file, automating its install, or crafting a Colab-friendly version for your report. You’re now primed for full-stack, cross-platform, reproducible AI deployment like a pro 🌐♻️🚀

📥 [Download the trained model](recycle_model.tflite)

---

🔗 [View the Recyclable Classifier on GitHub](https://github.com/leonardphokane/recyclable-classifier)

<p align="center">
  🔗 <a href="https://github.com/leonardphokane/recyclable-classifier">View the Recyclable Classifier on GitHub</a>
</p>
