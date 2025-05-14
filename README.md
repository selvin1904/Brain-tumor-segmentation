# Brain-tumor-segmentation
# 🧠 Brain Tumor Segmentation

A deep learning-based project for automatic segmentation of brain tumors from MRI scans. This tool assists medical professionals by accurately identifying and localizing brain tumor regions, aiding in diagnosis and treatment planning.

---

## 📌 Project Overview

This repository focuses on brain tumor segmentation using convolutional neural networks (CNNs), particularly U-Net architecture, which is widely used in biomedical image segmentation tasks.

---

## 📂 Dataset

The project is expected to use the *BraTS (Brain Tumor Segmentation)* dataset, a publicly available dataset that provides multi-modal MRI scans with pixel-level annotations for different tumor regions.

- *Modalities*: T1, T1Gd, T2, FLAIR
- *Labels*: Edema, Non-enhancing tumor core, Enhancing tumor

📎 [BraTS Dataset on Kaggle](https://www.kaggle.com/datasets/awsaf49/brats20-dataset-training-validation)

---

## 🏗️ Model Architecture

This project uses the *U-Net* architecture, which consists of:

- *Encoder*: Extracts features using convolutional layers and downsampling.
- *Decoder*: Reconstructs the image segmentation mask with upsampling.
- *Skip Connections*: Transfers high-resolution features from encoder to decoder.

The U-Net is ideal for medical imaging tasks due to its accuracy and efficiency in learning spatial features.

---

## 🧪 Training & Evaluation

### Training

- Input: Preprocessed MRI slices
- Augmentation: Random rotations, flips, brightness adjustments
- Loss Function: Dice Loss / Binary Cross-Entropy
- Optimizer: Adam

### 📊 Evaluation Metrics

- *Dice Similarity Coefficient (DSC)*
- *Intersection over Union (IoU)*
- *Accuracy / Precision / Recall*

---

## 🚀 Usage

1. *Clone the repository*
