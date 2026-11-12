# explainable-cervical-cell-classification
# Explainable AI Framework for Cervical Cell Diagnosis

## 1. Project Overview

This project focuses on cervical cell classification using **Multi-View Supervised Contrastive Learning** and Explainable Artificial Intelligence (XAI).

The objective is to classify cervical cell images into normal and abnormal categories while providing visual explanations to improve the interpretability of model predictions.

## 2. Dataset

- **Dataset:** Herlev Pap Smear Dataset
- **Total Images:** 917
- **Training Images:** 643
- **Test Images:** 274
- **Image Dimensions:** 128 × 128
- **Classification:** Normal and Abnormal

## 3. Technologies Used

- Python
- PyTorch
- ResNet18
- Deep Learning
- Computer Vision
- Grad-CAM
- Layer-wise Relevance Propagation (LRP)
- Image Segmentation
- OpenCV

## 4. Methodology

The project follows these major steps:

1. Dataset preparation and image preprocessing.
2. Image augmentation to generate multiple views.
3. Feature extraction using three ResNet18-based encoders.
4. Supervised contrastive learning for feature representation.
5. Classification using a hybrid loss combining contrastive loss and cross-entropy loss.
6. Explainability analysis using Grad-CAM and LRP.
7. Image segmentation for identifying relevant cellular regions.

## 5. Reported Results

| Evaluation Metric | Result |
|---|---:|
| Training Accuracy | 97.98% |
| Best Validation Accuracy Reported | 89.42% |
| Test Accuracy Reported | 91.61% |
| Precision | 92.01% |
| Recall | 91.61% |
| F1-Score | 91.17% |

**Evaluation note:** The notebook reuses the test data loader during validation and final evaluation. Therefore, the reported test accuracy should not be considered an independent holdout evaluation.

## 6. Explainable AI

The project incorporates:

- **Grad-CAM:** Visualizes image regions influencing model predictions.
- **LRP:** Helps understand the contribution of input features to predictions.
- **Image Segmentation:** Identifies relevant cellular regions for further analysis.


## 7. Project Files

- `MultiView.ipynb` – Implementation notebook containing the model and experimental workflow.
- `explainable-cervical-cell-classification.pdf` – Project presentation.

## 8. Limitations

- The dataset contains a relatively small number of images.
- Further evaluation using an independent test dataset is required.
- Additional validation is needed before considering real-world clinical applications.

