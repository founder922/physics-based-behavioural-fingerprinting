# Physics-Based Behavioural Fingerprinting

Dataset and software framework for industrial uptime verification using physics-based behavioural fingerprinting.

## Overview
This repository contains representative raw sensor excerpts, processed feature datasets, labels, metadata, and baseline scripts supporting the study of Dr Reji Kurien Thomas:
**A Cyber-Physical Software Architecture for Physics-Based Behavioural Fingerprinting in Industrial Uptime Verification**

## Repository Structure
- `raw_data/` - representative synchronised sensor excerpts
- `processed_data/` - segmented and feature-engineered datasets
- `labels/` - operational state labels
- `scripts/` - preprocessing, feature extraction, training, and evaluation scripts
- `metadata/` - sensor configuration and experiment details

## Experimental Setup
- Machine: Single-phase electric motor
- Runs: 5 repeated runs
- States: Active, Idle
- Vibration sampling: 1000 Hz
- Power sampling: 100 Hz (resampled into aligned excerpts for repository sharing)
- Window size: 1 second
- Overlap: 50%

## Processed Dataset
The `processed_data/features.csv` file contains **1000 labelled segments** with the following features:
- RMS vibration amplitude
- Dominant frequency (FFT)
- Spectral entropy
- Power variance
- Harmonic stability
- Acoustic RMS

## Important note
The raw CSV files in this repository are **representative public excerpts** designed to support reproducibility and repository usability.
They are aligned with the proof-of-concept setup reported in the paper.
