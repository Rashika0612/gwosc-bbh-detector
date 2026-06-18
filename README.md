# GWOSC BBH Detector And EM-GW

A deep-learning BBH detection pipeline trained on real GWOSC O3a noise.

## Features

- GWOSC O3a H1/L1 noise
- IMRPhenomD injections
- Welch PSD estimation
- Whitening
- Residual CNN architecture
- MixUp augmentation
- Label smoothing
- Early stopping

## Results

Test ROC-AUC: 0.889

TPR @ 1% FPR: 0.768

TPR @ 0.1% FPR: 0.740

Best F1: 0.866

## Future Work

- Multimessenger GW+EM detection
- NMMA/FiestaEM integration
- Parameter estimation

## Installation

```bash
git clone https://github.com/<username>/gwosc-bbh-detector.git
cd gwosc-bbh-detector

pip install -r requirements.txt
```
# GW-EM Multimessenger Detector

A multimessenger deep learning framework for joint gravitational-wave (GW) and electromagnetic (EM) transient detection.

## Overview

This project explores the use of multimodal neural networks for combining gravitational-wave strain data and optical light-curve information into a unified detection framework.

The GW branch uses real detector noise from the Gravitational Wave Open Science Center (GWOSC) together with simulated compact binary coalescence signals generated using IMRPhenomD waveforms. The EM branch processes synthetic kilonova-like light curves. Both modalities are encoded separately and fused into a joint classifier.

## Features

* Real GWOSC O3a detector noise (H1 and L1)
* IMRPhenomD waveform injections
* PSD estimation using Welch averaging
* Whitening and preprocessing pipeline
* Dual-branch GW + EM neural architecture
* Residual CNN feature extraction
* Data augmentation and label smoothing
* Multimessenger feature fusion
* ROC, Precision-Recall, and efficiency analysis

## Results

| Metric            | Value |
| ----------------- | ----- |
| ROC-AUC           | 0.940 |
| Average Precision | 0.963 |
| Best F1 Score     | 0.938 |
| TPR @ 1% FPR      | 0.883 |

These results demonstrate a significant improvement over the GW-only baseline detector and highlight the potential benefits of multimessenger information for transient classification.



