# Vesuvius Challenge – Scroll Surface Segmentation
  
This repository contains my work for the **Vesuvius Challenge**, where the goal is to develop a model capable of segmenting the **scroll surface** of carbonized Herculaneum papyri using 3D CT scan volumes. Effective surface tracing is a crucial step toward the virtual unwrapping and reading of ancient texts that have remained sealed for nearly two millennia.

---

## 🏛️ Project Overview

Ancient scrolls from the **Villa dei Papiri** were carbonized during the eruption of Mount Vesuvius in AD 79. Because these scrolls are too fragile to unroll physically, digital methods are used to recover their content.

This project focuses on:

* Detecting the **recto surface** (or an approximation of a sheet) within 3D CT volumes
* Avoiding **topological errors** such as merging separate sheets or introducing artificial holes
* Producing segmentation masks that can be directly integrated into the **Vesuvius digital unwrapping pipeline**

The output from this model helps the next stage—virtual unwrapping—extract and visualize text from the scrolls.

---

## 📦 Dataset Description

The dataset consists of 3D chunks of CT scans with binary labels. Key points:

* Captured at **ESRF (BM18)** and **DLS (I12)** synchrotrons
* Chunk sizes vary (non-fixed dimensions)
* A papyrus sheet includes:

  * **Recto**: horizontal fibers (target surface)
  * **Verso**: vertical fibers
* Labels identify the sheet surface; recto-specific detection is preferred but not required as long as sheet topology is preserved
* Additional datasets may be released during the competition (less curated)

---

## 🎯 Objective

To train a robust ML/DL model that:

* Accurately segments the papyrus sheet surface
* Handles noise, compression, folds, and tangled regions
* Produces topologically correct 3D masks ready for downstream unwrapping

---

## 🧠 Approach

This repository includes:

* Preprocessing scripts for CT chunks
* 3D model architectures (UNet3D / VNet / custom hybrid models)
* Training pipeline with mixed curated & semi-curated labels
* Sliding-window / patch-based inference
* Post-processing to remove artifacts & correct topology

---

## 🛠️ Tech Stack

* **Python**, **PyTorch**
* **3D CNNs**, UNet-based architectures
* **NumPy**, **SciPy**, **SimpleITK** for 3D volume handling
* **CUDA** acceleration for training
