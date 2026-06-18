# GWOSC BBH Detector

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
