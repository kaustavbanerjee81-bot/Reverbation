# Audio Reverberation Classification and Room Parameter Estimation

This project detects whether a speech signal is **clean** or **reverberant** from 1 bit quantised signals and estimates room acoustic parameters from quantized speech using machine learning and deep learning models.

## Pipeline

1. Load clean speech from the **TIMIT** dataset.
2. Simulate room reverberation using **PyRoomAcoustics**.
3. Quantize speech into different bit depths (1, 2, 4, 8, and 16-bit).
4. Extract acoustic features:
   - Zero Crossing Rate (ZCR)
   - Autocorrelation
   - Spectral Centroid
   - Spectral Rolloff
   - Spectral Entropy
   - Spectral Flatness
5. Train ML models (SVM, Random Forest, Logistic Regression, KNN, Gradient Boosting, Naive Bayes) and CNN models.
6. Classify speech as **Clean** or **Reverberant** and estimate room acoustic parameters.

## Technologies

- Python
- NumPy
- Librosa
- PyRoomAcoustics
- Scikit-learn
- TensorFlow / PyTorch

## Applications

- Speech Enhancement
- Audio Signal Processing
- Room Acoustic Analysis
- Reverberation Detection
- Speech Recognition

## Repository Structure

```
data/
preprocessing/
feature_extraction/
models/
training/
evaluation/
results/
README.md
```

## Author

**Kaustav Banerjee**  
Department of Electrical Engineering  
Indian Institute of Science (IISc), Bangalore
