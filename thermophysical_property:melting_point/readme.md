# Melting Point Prediction Challenge
      
## 🧪 Overview

The goal of this project is to build machine learning models that predict the melting point (°C) of organic compounds using molecular descriptors. Melting point is a critical property in chemistry, impacting drug design, material selection, and process safety. However, obtaining experimental melting point data is often expensive, time-consuming, or not always feasible.

In this challenge, you’ll leverage group contribution features—subgroup counts that represent functional groups within each molecule—to capture complex, nonlinear relationships between molecular structure and melting behavior.

The performance of models is evaluated using **Mean Absolute Error (MAE)** on a held-out test set. The lower the MAE, the better the model’s predictions.

---

## 📊 Dataset

- **Total compounds**: 3,328  
- **Training set**: 2,662 samples (80%)  
- **Test set**: 666 samples (20%)  
 
### Files:
- `train.csv` : Includes features and target (melting point, `Tm`)
- `test.csv` : Contains features only, without target
- `sample_submission.csv` : Template submission file with columns `id` and `Tm`

### Columns:
- `id` : Unique identifier for each sample
- `SMILES` : Simplified molecular-input line-entry system string representation of the molecule
- `Group 1..N` : Descriptor features representing functional groups within the molecule
- `Tm` : Melting point in Kelvin (only in the training set)
- 
