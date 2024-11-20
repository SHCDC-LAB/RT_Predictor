# Retention Time Prediction Using Transfer Learning

This repository provides tools and models for predicting retention times (RT) of chemical compounds, focusing on hazard identification. The project leverages transfer learning and extensive datasets to enhance the accuracy of RT prediction for a wide variety of molecules, including pesticides, veterinary drugs, and environmental phenols.

---

## Overview

### 1. Source Domain Model
- **Input Data**: Electrospray Ionization (ESI, positive mode) data from 823 molecules.
- **Dataset Composition**:
  - Pesticides and pesticide transformed products
  - Veterinary drugs
  - Sunscreens
  - Environmental phenols
  - PFAS
  - Antiseptic

### 2. Transfer Learning
- **Training Data**: ESI (negative mode) data from 325 molecules.
- **Application**: Enhanced RT prediction for diverse compounds.

### 3. Prediction Data
- **Pesticide Transformation Products**:
  - 1,247 molecules
  - Reference: [PMID: 31450217](https://doi.org/10.1016/j.watres.2019.114972)
- **Mass Spectrometry Databases**:
  - MassBank: 100,000+ spectra ([MassBank-data](https://github.com/MassBank/MassBank-data/releases/latest))
  - MzCloud: 8,990+ spectra ([MzCloud](https://www.mzcloud.org/))
- **Human Exposure Compounds**:
  - 17,400+ prioritized compounds
  - Reference: [PMID: 33929905](https://doi.org/10.1289/EHP7722), [PMC: PMC8086799](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC8086799/)

### 4. Application
- Hazardous substance identification using RT prediction.

---

## Features

- **Transfer Learning Model**: A robust model trained on ESI (-) mode data, adapting knowledge from ESI (+) mode.
- **RT Prediction Pipeline**:
  - Predict RTs for large-scale datasets.
  - Supports diverse compound libraries, including pesticide transformation products and human exposure chemicals.

---

## Files and Directories

- `MolecularFeature_generation.ipynb`: Notebook for feature extraction and data preparation.
- `TransferLearning_model_Prediction.ipynb`: Notebook for training the transfer learning model and making predictions.

---

## Installation

1. Clone this repository:
   ```bash
   git clone https://github.com/SHCDC-LAB/RT_Predictor.git
