# Physics-Based Behavioural Fingerprinting

## Overview
This repository contains the dataset, preprocessing pipeline, feature extraction scripts, and model implementation used for the study:

**A Cyber-Physical Software Architecture for Physics-Based Behavioural Fingerprinting in Industrial Uptime Verification**

The objective is to enable independent verification of machine uptime by comparing software-reported activity with physically observed behaviour using sensor signals.

---

## Repository Structure

- raw_data/ → original sensor recordings  
- processed_data/ → segmented and feature datasets  
- labels/ → operational state labels  
- scripts/ → preprocessing and ML pipeline  
- metadata/ → sensor configuration and experiment details  
- figures/ → supporting figures  

---

## Experimental Setup

- Machine: Single-phase electric motor  
- Runs: 5  
- Duration: ~10 minutes per run  
- States: Active, Idle  
- Vibration sampling: 1000 Hz  
- Power sampling: 100 Hz  
- Window size: 1 second  
- Overlap: 50%  

---

## Features Extracted

- RMS vibration amplitude  
- Dominant frequency (FFT)  
- Spectral entropy  
- Power variance  

---

## Model

Random Forest classifier with:
- 100 trees  
- max depth = 10  
- 70/30 train-test split  
- 5-fold cross-validation  

---

## Reproducibility

Steps:

1. Run preprocessing  
2. Extract features  
3. Train model  
4. Evaluate results  

---

## Data Availability

The dataset and scripts will be released publicly upon publication.  
A DOI-linked archive will be created for long-term reproducibility.

---

## License

MIT License
