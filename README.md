# Undergraduate-Research-Programme
Detecting Parkinsons Disease With Images 
# Parkinson's Disease Detection Using VGG19 and ResNet

This repository contains our undergraduate research implementation for detecting **Parkinson’s Disease (PD)** from medical imaging using **Convolutional Neural Networks (CNNs)** — specifically **VGG19** and **ResNet** architectures.

Our work focuses on applying deep learning models to MRI and SPECT DaTscan images to distinguish Parkinson’s patients from healthy individuals.

---

## Project Objectives

- Apply **VGG19** and **ResNet** deep learning architectures for PD detection.
- Perform **data preprocessing** to enhance MRI/SPECT image quality.
- Train and evaluate models to measure accuracy, precision, recall, and F1-score.
- Compare performance of VGG19 and ResNet to determine the most effective CNN model for medical diagnosis.

---

## Dataset

We used datasets containing **T1-weighted MRI** and **SPECT DaTscan** images:
- NTUA Parkinson MRI Dataset [🔗 GitHub Link](https://github.com/ails-lab/ntua-parkinson-dataset)
- Public access PPMI DaTscan data (for SPECT imaging)

Due to data privacy and size constraints, the dataset is not uploaded here. Please follow the dataset links and instructions for access.

---

## Models Implemented

### VGG19
- A deep 19-layer CNN pre-trained on ImageNet.
- Fine-tuned on Parkinson’s image dataset.
- Applied transfer learning and modified final layers for binary classification.

### ResNet
- Deep residual network (ResNet-50).
- Used skip connections to avoid vanishing gradient issues.
- Also fine-tuned with frozen layers and custom dense layers.

---

## Repository Structure

