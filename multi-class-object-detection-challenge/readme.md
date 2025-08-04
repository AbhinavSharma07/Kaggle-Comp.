# Multi-Class Object Detection Challenge 🚀

Welcome to the next evolution of the Synthetic-to-Real Object Detection Challenge - now a multi-class detection task co-hosted by Duality AI and 3LC.

## 🏆 Challenge Summary

**Your Goal:**
Build an object detection model that can identify multiple classes (Soup + Cheerios) in real-world test images, using only synthetic data that you generate through FalconCloud, Duality’s high-fidelity digital twin simulation platform.

But that’s not all! This time, we’re introducing a brand new collaborative workflow with 3LC, a cutting-edge platform for identifying failure modes in AI systems. After training your model on synthetic data, you’ll use 3LC’s tools to analyze your model’s blind spots, then head back to FalconCloud to generate additional targeted data to fix them. It’s an iterative, intelligent approach to training models that work in the real world.

- 👉 [Watch a competition overview video on FalconCloud](#)
- 👉 [Watch a competition overview video on 3LC](#)

## 🌟 What’s New in This Challenge?

- **Two object classes:** Cheerios + Soup
- **Two data generation modes:**
  - Randomized data scenario: for rapid prototyping and large datasets
  - Targeted capture mode: click to collect synthetic data from specific camera angles and drop locations for specialized data
- **Built-in model debugging:** Use 3LC to find gaps in model training & data quality
- **Iterative feedback loop:** Diagnose → Generate → Retrain → Repeat

## 🧠 Learn the Real-World Workflow

In this challenge, you’ll follow a simulation-to-deployment pipeline used by actual AI engineering teams:

1. Generate synthetic training data using FalconCloud
2. Train an object detection model using 3LC (YOLOv8 recommended)
3. Analyze model performance on a per-sample basis in 3LC Dashboard
4. Identify weaknesses in your model such as persistent false positives or false negatives
5. Collect more data from the Falcon scenario to address those gaps
6. Repeat the process to achieve the highest mAP@50

This mimics the workflow used in fields like robotics, manufacturing QA, and autonomous systems - where collecting real-world data is expensive and iterative simulation is key.

## 🛠️ Setup and Installation

### Prerequisites

- Python 3.8 or higher
- PyTorch
- Ultralytics YOLOv8
- Ensemble-boxes

