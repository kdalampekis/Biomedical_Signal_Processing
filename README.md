# 🧠 EEG Classification using CSP and Machine Learning

This notebook implements a full EEG signal processing and classification pipeline based on the **EEGBCI dataset**, focused on **motor imagery** tasks.

It includes:
- Preprocessing EEG signals using the `MNE` library
- Selecting and renaming motor-related event annotations
- Extracting spatial features using **Common Spatial Patterns (CSP)**
- Applying machine learning classifiers (e.g. LDA, SVM) to detect motor intentions

---

## 🎯 Objectives

- Understand EEG signal characteristics and preprocessing needs
- Learn how to extract discriminative features for brain-computer interfaces (BCI)
- Compare classification performance for left/right hand, fists/feet motor imagery
- Handle EEG data from multiple subjects using standardized MNE pipelines

---

## 📂 Project Structure

- `Copy_of_eeg_classification_v2-1.ipynb`: Main notebook containing all preprocessing, feature extraction, training, and evaluation steps
- **EEG Data**: Loaded directly using `mne.datasets.eegbci` from PhysioNet
- **Preprocessing**: Includes filtering, channel selection, and epoch segmentation
- **Feature Extraction**: Performed via Common Spatial Patterns (CSP)
- **Classification**: Evaluated with LDA and optionally SVM

---

## 📊 Features

- Motor imagery detection for:
  - Left hand
  - Right hand
  - Both fists
  - Both feet
- Visualizations of EEG signal characteristics and classification results
- Accuracy evaluation across different runs/subjects

---

## 🛠️ Technologies Used

- Python 3
- [MNE-Python](https://mne.tools/stable/index.html)
- NumPy, Pandas
- scikit-learn
- Matplotlib, Seaborn
- Google Colab / Jupyter Notebook

---

## ▶️ How to Run

1. Open the notebook in **Google Colab** or locally in **Jupyter Notebook**.
2. Make sure the following libraries are installed:

```bash
pip install mne numpy pandas scikit-learn matplotlib seaborn
