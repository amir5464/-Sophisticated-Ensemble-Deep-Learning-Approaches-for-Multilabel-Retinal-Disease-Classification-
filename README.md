# Sophisticated Ensemble Deep Learning Approaches for Multilabel Retinal Disease Classification

[![License: CC BY 4.0](https://img.shields.io/badge/License-CC%20BY%204.0-lightgrey.svg)](https://creativecommons.org/licenses/by/4.0/)

## 📄 Paper Info

**Title:** Sophisticated Ensemble Deep Learning Approaches for Multilabel Retinal Disease Classification in Medical Imaging  
**Authors:** Asghar Amir, Tariqullah Jan, Mohammad Haseeb Zafar, Shadan Khan Khattak  
**Published In:** CAAI Transactions on Intelligence Technology (2025)  
**DOI:** [10.1049/cit2.70012](https://doi.org/10.1049/cit2.70012)

## 📌 Abstract

This work presents an advanced multi-label retinal disease classification system using ensemble deep learning. The proposed model employs a stacking ensemble approach, combining DenseNet201, EfficientNetB3/B4/V2S, and uses Logistic Regression and deep learning as meta-models.

Key results:
- **Accuracy:** 93.5%
- **Precision:** 98.2%
- **Recall:** 93.9%
- **F1 Score:** 96%
- **Loss:** 0.029

## 🧠 Methodology Overview

### 🔹 Dataset
- **RFMiD** (Retinal Fundus Multi-disease Image Dataset)
- 3200 fundus images
- 46 disease labels
- Expert-labeled and stratified split

### 🔹 Models Used
- **Binary Classifier:** DenseNet201 & EfficientNetV2S
- **Multi-label Classifier:** EfficientNetB3, B4, V2S (weighted & unweighted)
- **Meta-models:** Neural Network & Logistic Regression

### 🔹 Preprocessing
- Cropping and resizing (Alpha, Beta, Gamma strategies)
- Data augmentation (flip, brightness, hue, etc.)
- Class balancing via upsampling

### 🔹 Ensemble Strategy
- **Stacking Ensemble**:
  - Base learners: CNN architectures
  - Meta-learners: DNN and Logistic Regression
- Separate ensembles for binary detection and multi-label classification
- Final prediction combines both outputs

## 📈 Performance Summary

| Model                          | Accuracy | Precision | Recall | F1 Score | AUC  | mAP  |
|-------------------------------|----------|-----------|--------|----------|------|------|
| DenseNet201 (binary)          | 95.4%    | 98.0%     | 96.2%  | 97.1%    | 0.989| -    |
| EfficientNetV2S (binary)      | 95.9%    | 98.5%     | 96.2%  | 97.4%    | 0.988| -    |
| Final Stacking Ensemble       | 93.5%    | 98.2%     | 93.9%  | 96.0%    | 0.992| 0.960|
| EfficientNetB4 (w/o weights)  | 86.2%    | 98.4%     | 95.5%  | 96.6%    | 0.996| 0.984|
| EfficientNetV2S (w/ weights)  | 85.7%    | 98.0%     | 93.6%  | 95.4%    | 0.995| 0.980|

## 📊 Evaluation Metrics
- Accuracy
- Precision, Recall, F1-Score
- Hamming Loss
- AUC (ROC & PR)
- Mean Average Precision (mAP)

## 📁 Dataset

Dataset used in this study is available on [Kaggle](https://www.kaggle.com/datasets/andrewmvd/retinal-disease-classification).

## 📚 Citation

If you use this work, please cite it as:

```bibtex
@article{amir2025sophisticated,
  title={Sophisticated Ensemble Deep Learning Approaches for Multilabel Retinal Disease Classification in Medical Imaging},
  author={Amir, Asghar and Jan, Tariqullah and Zafar, Mohammad Haseeb and Khattak, Shadan Khan},
  journal={CAAI Transactions on Intelligence Technology},
  year={2025},
  publisher={Wiley Online Library}
}
