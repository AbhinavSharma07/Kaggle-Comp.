# 🩻 Grand X-Ray Slam: Division A
 
Welcome to the official repository for our participation in the **Grand X-Ray Slam: Division A**, a Kaggle Community Hackathon focused on building life-saving AI models for thoracic disease detection from chest X-rays.

---

## 📌 Overview

**Grand X-Ray Slam: Division A** is the first of a two-part competition series on Kaggle, aimed at advancing medical imaging through artificial intelligence. Participants are challenged to develop multi-label classification models capable of detecting 14 different thoracic conditions from chest radiographs.

This challenge supports **Dr HealthAgent**, a personal health app developed by **Blue and Gold Healthcare Inc.**, to enhance global access to medical diagnostics.

---

## 🧠 Problem Statement

Build AI models to identify the following **14 thoracic conditions** in chest X-ray images:

- Atelectasis  
- Cardiomegaly  
- Consolidation  
- Edema  
- Enlarged Cardiomediastinum  
- Fracture  
- Lung Lesion  
- Lung Opacity  
- No Finding  
- Pleural Effusion  
- Pleural Other  
- Pneumonia  
- Pneumothorax  
- Support Devices  

This is a **multi-label classification** task—each X-ray image may contain **none, one, or multiple conditions**.

---

## 🗂️ Dataset

- **Train Set**: 107,374 images (~138 GB)  
- **Test Set**: 46,233 images (~60 GB)  
- **Source**: De-identified chest X-rays from multiple healthcare institutions  
- **Format**: Images with associated condition labels (multi-label binary format)

---

## 🧰 Tech Stack

- **Framework**: PyTorch / TensorFlow (Choose based on your implementation)  
- **Model Architectures**: CNNs (e.g., ResNet, EfficientNet), Transformers (e.g., ViT)  
- **Training**: Multi-label loss functions (e.g., BCEWithLogitsLoss)  
- **Evaluation Metric**: Mean AUROC across 14 classes  
- **Augmentation**: Albumentations / torchvision.transforms  
- **Experiment Tracking**: Weights & Biases / TensorBoard  
