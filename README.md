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

## Results Summary

Below are the performance metrics of our implemented models, evaluated on the test set containing 4,401 images (1,071 Non-PD, 3,330 PD cases):

| Model   | Accuracy | Precision | Recall | F1-Score |
|---------|----------|-----------|--------|----------|
| VGG19   | 98.0%    | 96% / 99% | 96% / 99% | 96% / 99% |
| ResNet50| 98.0%    | 95% / 99% | 97% / 98% | 96% / 99% |

> - **VGG19** showed strong performance, especially in identifying PD patients with high precision and recall (0.99).
> - **ResNet50** achieved slightly better generalization, with balanced performance across both classes.

- **Macro Avg F1-Score (VGG19):** 0.97  
- **Macro Avg F1-Score (ResNet50):** 0.97  
- **Weighted Avg Accuracy (Both):** 0.98

---

## 📌 Future Work

- Experiment with **model ensembling** of VGG19 and ResNet to further improve performance.
- Integrate **optimization algorithms** like **Grey Wolf Optimization (GWO)** for tuning hyperparameters.
- Explore other deep learning architectures (e.g., Inception, DenseNet).
- Deploy the trained models as part of a diagnostic **web app using Flask or Streamlit**.

---

## 👨‍💻 Team

- **Gokul Nandan** (E22CSEU1739)  
- **Vamsh Reddy** (E22CSEU0838)  
- **Karkala Vignesh Reddy** (E22CSEU1695)  

---

## 📚 References

Please refer to our full research document for complete citations. Some key datasets and sources used:
- NTUA Parkinson Dataset: [https://github.com/ails-lab/ntua-parkinson-dataset](https://github.com/ails-lab/ntua-parkinson-dataset)
- Michael J. Fox Foundation on Parkinson’s: [https://www.michaeljfox.org](https://www.michaeljfox.org)
- Parkinson’s Progression Markers Initiative (PPMI): [https://www.ppmi-info.org](https://www.ppmi-info.org)

---

## 📜 License

This repository is maintained for academic and educational use only.  
Contact us for permission regarding reuse, extension, or deployment.

---

