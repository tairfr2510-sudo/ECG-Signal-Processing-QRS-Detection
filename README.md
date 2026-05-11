# Biomedical Signal Processing: ECG Analysis & QRS Detection

## Overview
This repository contains a robust implementation for processing and analyzing Electrocardiogram (ECG) signals using MATLAB. The project focuses on automated feature extraction, specifically the detection of the QRS complex, which is a critical step in heart rate monitoring and clinical diagnostics.

The methodologies used here, such as digital filtering and peak detection algorithms, are highly relevant to other physiological signals like EEG.

## Key Features
* **Signal Preprocessing:** Implementation of Band-pass filters to remove common artifacts such as power-line interference (50/60Hz) and baseline wander.
* **QRS Detection Algorithm:** A derivative-based approach to accurately identify R-peaks in real-time or offline recordings.
* **Feature Extraction:** Automated calculation of Heart Rate (BPM) and Heart Rate Variability (HRV) metrics.
* **Data Visualization:** Clear plotting of raw vs. filtered signals with identified peaks for verification.



## Technical Implementation
1.  **Loading Data:** The system processes `.mat` files containing raw physiological data.
2.  **Filtering:** Applying digital signal processing (DSP) techniques to enhance the signal-to-noise ratio (SNR).
3.  **Peak Identification:** Utilizing thresholding and local maxima search to locate the QRS complexes.

## File Structure
* `ECG_QRS_Detection_Analysis.m`: Main MATLAB script containing the processing pipeline.
* `/data`: Directory containing sample ECG recordings (`ecg1.mat`, `ecg2.mat`).
* `/results`: Pre-calculated peak indices for validation.

## How to Use
1.  Clone this repository: `git clone https://github.com/YOUR_USERNAME/ECG-Signal-Processing.git`
2.  Open MATLAB and navigate to the project folder.
3.  Run the main script: `ECG_QRS_Detection_Analysis.m`.
4.  View the generated plots and heart rate metrics in the Command Window.

## Future Improvements
* Integration with Real-time Signal Acquisition systems.
* Implementation of Wavelet Transform for enhanced noise reduction.
* Porting the algorithm to Python (NumPy/SciPy) for broader integration.

---
*Developed by Tair Fridman as part of Biomedical Engineering studies at the Technion.*
