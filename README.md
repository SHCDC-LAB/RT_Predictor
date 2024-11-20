Retention Time Prediction Using Transfer Learning

This repository provides tools and models for predicting retention times (RT) of chemical compounds, focusing on hazard identification. The project leverages transfer learning and extensive datasets to enhance the accuracy of RT prediction for a wide variety of molecules, including pesticides, veterinary drugs, and environmental phenols.

Overview
Source Domain Model:

Input Data: Electrospray Ionization (ESI, positive mode) data from 823 molecules.
Dataset Composition:
Pesticides
Veterinary drugs
Sunscreens
Environmental phenols
Transfer Learning:

Training Data: ESI (negative mode) data from 325 molecules.
Application: Enhanced RT prediction for diverse compounds.
Prediction Data:

Pesticide Transformation Products:
1,247 molecules
Reference: PMID: 31450217
Mass Spectrometry Databases:
MassBank: 100,000 spectra (MassBank-data)
MzCloud: 8,990 spectra (MzCloud)
Human Exposure Compounds:
17,400+ prioritized compounds
Reference: PMID: 33929905, PMC: PMC8086799
Application:

Hazardous substance identification using RT prediction.
Features
Transfer Learning Model: A robust model trained on ESI (-) mode data, adapting knowledge from ESI (+) mode.
RT Prediction Pipeline:
Predict RTs for large-scale datasets.
Supports diverse compound libraries, including pesticide transformation products and human exposure chemicals.
Files and Directories
MolecularFeature_generation.ipynb: Notebook for feature extraction and data preparation.
TransferLearning_model_Prediction.ipynb: Notebook for training the transfer learning model and making predictions.
Usage
Feature Extraction: Run MolecularFeature_generation.ipynb to preprocess the input data and generate features for model training.

Training and Prediction: Use TransferLearning_model_Prediction.ipynb to:

Train the RT prediction model using transfer learning.
Predict RTs for the specified datasets.
Results Analysis: Evaluate the RT prediction results to identify hazardous substances.
