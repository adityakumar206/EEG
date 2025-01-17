EEG Classification Model

Overview
This project focuses on classifying EEG signals to distinguish between normal and epileptic brain states. Using two datasets—CHB-MIT EEG Dataset and Bonn EEG Dataset—we preprocess, extract features, and train machine learning models to achieve accurate classification. The results offer insights into how EEG signals can be used to support the diagnosis and management of epilepsy.

Objectives
Preprocess EEG signals to reduce noise and standardize data.
Extract meaningful statistical features for analysis.
Build and train classification models:
Neural Network for CHB-MIT EEG Dataset.
Random Forest for Bonn EEG Dataset.
Evaluate models using appropriate metrics and visualize results.

Datasets
1. CHB-MIT EEG Dataset
Source: MIT's CHB-MIT database.
Format: EDF files.
Use: Focused on distinguishing between seizure and non-seizure signals.
2. Bonn EEG Dataset
Source: Bonn University's dataset.
Format: Text files.
Use: Classified EEG signals into normal and epileptic states.

Methodology
CHB-MIT EEG Dataset
Preprocessing: Low-pass Butterworth filter applied to remove high-frequency noise.
Feature Extraction: Statistical measures like mean, standard deviation, etc.
Model: Neural Network with the Adam optimizer and binary cross-entropy loss.
Evaluation: Measured performance using accuracy and loss metrics.
Visualization: Plotted training vs. validation accuracy and scatter plots for predictions.
Bonn EEG Dataset
Preprocessing: Normalized data to a range of 0-1.
Feature Extraction: Statistical features like median, variance, etc.
Model: Random Forest for robust classification.
Evaluation: Measured accuracy, precision, recall, and F1-score.
Visualization: Confusion matrix and box plots for feature distribution.


Results
CHB-MIT Dataset:

Neural Network successfully classified seizure and normal EEG signals.
Training and validation accuracies visualized over epochs.
Bonn Dataset:

Random Forest achieved high accuracy in classifying EEG signals.
Confusion matrix and feature distribution confirmed model robustness.


Tools and Libraries
Data Processing: numpy, pandas, pyedflib
Visualization: matplotlib, seaborn
Modeling: sklearn, keras
