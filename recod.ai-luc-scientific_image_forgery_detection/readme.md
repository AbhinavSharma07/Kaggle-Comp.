
# 🧬 Scientific Image Copy-Move Forgery Detection

<p align="center">
  <strong>Protecting scientific integrity — one pixel at a time</strong>
</p>

<p align="center">
  <img src="https://img.shields.io/badge/Domain-Biomedical%20Imaging-blue"/>
  <img src="https://img.shields.io/badge/Task-Copy--Move%20Forgery%20Detection-red"/>
  <img src="https://img.shields.io/badge/Output-Pixel--Level%20Segmentation-green"/>
  <img src="https://img.shields.io/badge/Status-Research%20Project-purple"/>
</p>

---

## 🚀 Overview

Scientific images are a cornerstone of published research — yet not all are trustworthy.

This project focuses on **detecting and segmenting copy-move forgeries in biomedical images**, a common form of scientific misconduct where parts of an image are duplicated to fabricate or exaggerate experimental results.

Manual inspection by reviewers is slow and unscalable. Generic image-forensics tools struggle with the complexity of biomedical figures.  
**This project aims to change that.**

---

## 🧠 What is Copy-Move Forgery?

<details>
<summary><strong>Click to expand</strong></summary>

Copy-move forgery occurs when:
- A region of an image is copied
- The copied region is pasted elsewhere **within the same image**
- The intent is to hide, duplicate, or fabricate scientific evidence

In biomedical research, this can include:
- Duplicated microscopy regions
- Reused Western blot bands
- Manipulated cell or tissue images

These manipulations are often subtle and hard to spot with the naked eye.

</details>

---

## 📌 Problem Statement

Current approaches fail because:

- 🐢 **Manual review** is slow and inconsistent  
- 🧰 **Generic forensic tools** aren’t designed for scientific images  
- 🔬 **Biomedical images** have complex textures and artifacts  
- 🧩 **Multi-panel figures** confuse traditional detectors  

We need a **domain-specific, scalable, automated solution**.

---

## 📊 Dataset

<details>
<summary><strong>Dataset Highlights</strong></summary>

- ✔️ Several hundred **confirmed copy-move forgeries**
- ✔️ Extracted from **2,000+ retracted scientific papers**
- ✔️ **Pixel-level annotations** of copied regions
- ✔️ Multiple biomedical imaging modalities

This is one of the **most realistic and detailed datasets** available for scientific image forensics.

</details>

---

## 🎯 Objective

Build machine learning models that can:

- 🔍 Detect whether an image contains copy-move forgery  
- 🧩 Segment duplicated regions **at pixel level**  
- 🔄 Generalize across biomedical image types  

📐 **Evaluation focuses on segmentation accuracy**, emphasizing precise localization of forged regions.

---

## 🧪 Expected Impact

A successful model can:

- 🧾 Assist journals in pre-publication screening  
- 👩‍🔬 Support reviewers and research institutions  
- 💰 Save time, funding, and research credibility  
- 🛡️ Reduce the spread of fraudulent scientific results  

**Goal:** Strengthen trust in published biomedical research.
