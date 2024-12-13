# EEG-Based-Detection-of-Intellectual-Development-Disorder
## Introduction
Electroencephalography (EEG) provides a non-invasive way to study brain activity. This project applies statistical, spectral, and temporal feature extraction to EEG data for the classification of healthy and affected individuals.

---

## Features
This project extracts the following features from EEG signals:

1. **Statistical Features:**
   - Mean
   - Standard Deviation
   - Variance
   - Skewness
   - Kurtosis
   - Median
   - Interquartile Range (IQR)

2. **Temporal Features:**
   - Peak-to-Peak Amplitude (PTP)
   - Root Mean Square (RMS)
   - Absolute Signal Difference
   - Zero-Crossing Rate

3. **Spectral Features:**
   - Power Spectral Density (PSD) Mean
   - Dominant Frequency
   - Spectral Entropy

---

## Data Preprocessing
1. **Loading EEG Data**: EEG data files are loaded in the `.edf` format.
2. **Preprocessing**:
   - EEG signals are referenced to the average.
   - Bandpass filtering is applied (1-45 Hz).
   - Signals are segmented into epochs (25 seconds).

3. **Labels**:
   - Healthy individuals are labeled as `0`.
   - Patients are labeled as `1`
