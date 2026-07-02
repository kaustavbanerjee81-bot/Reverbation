# Reverbation
# Audio Reverberation Classification and Room Parameter Estimation

This project focuses on detecting reverberation in speech recordings and estimating room acoustic parameters using machine learning and deep learning.

The goal is to determine whether a speech signal is **clean** or **reverberant**, even after heavy signal quantization such as **1-bit speech**. The project also explores predicting room characteristics from reverberant speech.

---

## Project Overview

When speech is recorded inside a room, reflections from walls, ceilings, and floors create **reverberation**. These reflections reduce speech quality and affect applications like:

- Speech Recognition
- Speaker Identification
- Hearing Aids
- Audio Enhancement

This project investigates whether reverberation information is still present after aggressive signal quantization and whether it can be used for classification and room analysis.

---

## Features

- Reverberation Detection
- Clean vs Reverberant Speech Classification
- Room Acoustic Parameter Estimation
- 1-bit and Multi-bit Quantized Speech Analysis
- Machine Learning and Deep Learning Models
- Feature Extraction from Speech Signals

---

## Dataset

This project uses the **TIMIT Speech Corpus**.

The dataset is split into:

- Training Set
- Validation Set
- Test Set

Speaker-level splitting is used to prevent data leakage.

---

## Data Processing Pipeline

```
Clean Speech
      │
      ▼
Room Simulation
      │
      ▼
Reverberant Speech
      │
      ▼
Signal Quantization
      │
      ▼
Feature Extraction
      │
      ▼
Machine Learning / Deep Learning
      │
      ▼
Prediction
```

---

## Features Extracted

Some of the extracted features include:

- Zero Crossing Rate (ZCR)
- Autocorrelation
- Long-Term Temporal Correlation (LTTC)
- Spectral Centroid
- Spectral Rolloff
- Spectral Entropy
- Spectral Flatness

---

## Models Used

### Machine Learning

- Support Vector Machine (SVM)
- Random Forest
- Logistic Regression
- K-Nearest Neighbors (KNN)
- Gradient Boosting
- Naive Bayes

### Deep Learning

- 1D Convolutional Neural Network (1D CNN)
- 2D Convolutional Neural Network (2D CNN)

---

## Results

The project compares several feature combinations and classifiers.

Highlights include:

- ZCR alone provides limited performance.
- Combining temporal and spectral features significantly improves accuracy.
- Deep learning models achieve the best performance.
- The 2D CNN achieved approximately **95% test accuracy**.

---

## Technologies Used

- Python
- NumPy
- SciPy
- Librosa
- PyRoomAcoustics
- Scikit-learn
- TensorFlow / PyTorch
- Matplotlib

---

## Repository Structure

```
├── data/
├── preprocessing/
├── feature_extraction/
├── models/
├── training/
├── evaluation/
├── notebooks/
├── results/
├── README.md
└── requirements.txt
```

---

## Applications

- Speech Enhancement
- Blind Reverberation Detection
- Room Acoustic Analysis
- Audio Signal Processing
- Machine Learning for Speech
- Deep Learning for Audio

---

## Future Work

- Predict additional room acoustic parameters (RT60, DRR, C50, C80).
- Improve robustness in noisy environments.
- Train on larger and more diverse speech datasets.
- Explore transformer-based audio models.
- Develop real-time reverberation detection systems.

---

## Author

**Kaustav Banerjee**

Department of Electrical Engineering  
Indian Institute of Science (IISc), Bangalore

---

## License

This project is intended for academic and research purposes.
