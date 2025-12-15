# 🌱 Pasture Biomass Prediction

Predict pasture biomass from images, ground-truth measurements, and public datasets to support smarter grazing decisions for farmers.

---

## 📌 Overview

Accurately estimating pasture biomass is critical for sustainable grazing management. Traditional methods like *clip-and-weigh* are accurate but slow and impractical at scale, while sensor-based tools can be unreliable in diverse field conditions.

This project builds machine learning and deep learning models that estimate pasture biomass using:

* Ground-based pasture images
* Ground-truth biomass measurements
* NDVI and other publicly available environmental datasets

The goal is to provide scalable, reliable biomass estimation to improve livestock welfare, pasture health, and farm productivity.

---

## 🎯 Objectives

* Predict pasture biomass (kg DM/ha) from images
* Leverage NDVI and auxiliary environmental data
* Generalize across seasons, regions, and species mixes
* Enable decision-making for grazing timing and intensity

---

## 📂 Dataset

The dataset includes:

* 📷 RGB pasture images (field-level)
* 📏 Ground-truth biomass measurements
* 🌍 Metadata (location, season, pasture type)
* 🌿 NDVI values for vegetation health

> Data spans multiple Australian regions and seasons with professionally annotated labels.

---

## 🧠 Approach

* Image-based feature extraction using CNNs (e.g., ResNet, EfficientNet)
* Fusion of visual features with NDVI and tabular data
* Regression-based learning for biomass prediction
* Evaluation using RMSE, MAE, and R² metrics

---

## 🛠️ Tech Stack

* **Language:** Python 3.11+
* **Deep Learning:** PyTorch / TensorFlow
* **ML:** scikit-learn
* **Image Processing:** OpenCV, torchvision
* **Data Handling:** NumPy, Pandas
* **Visualization:** Matplotlib, Seaborn

---

## 📊 Results

* Robust performance across seasonal and regional variation
* Improved accuracy over traditional meter-based estimates
* Demonstrates strong potential for real-world farm deployment

---

## 🌾 Impact

* Smarter grazing and pasture recovery decisions
* Reduced overgrazing and feed wastage
* Better animal welfare and long-term soil health
