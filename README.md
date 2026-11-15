# Hack4Hack 2026 – Planet Hunters

## Overview
This repository contains my Round 1 hackathon work for **Hack4Hack 2026 – Planet Hunters**.

The project focuses on centroid analysis and machine learning-based evaluation to support the classification of astronomical objects.

## Problem Focus
The notebook explores spatial centroid time-series data to extract useful features that can help distinguish between different astronomical classes, with particular attention to background binary identification and pointing-related anomalies.

## My Work: Centroid Analysis & Model Evaluation

The notebook implements the following:

- **Centroid Feature Extraction:** Extracts statistical and spatial features from X and Y centroid time series.
- **Statistical Analysis:** Calculates mean, median, standard deviation, IQR, skewness, kurtosis and displacement metrics.
- **Memory-Efficient Processing:** Uses chunk-based processing and NumPy memory mapping to handle large datasets.
- **Machine Learning:** Implements LightGBM multiclass classification with a HistGradientBoostingClassifier fallback.
- **Model Evaluation:** Uses stratified 5-fold cross-validation.
- **Performance Metrics:** Evaluates Macro F1-score, accuracy, classification reports and confusion matrices.
- **Class-Specific Analysis:** Includes precision, recall and F1 evaluation for the background_binary class.

## Technologies Used

- Python
- NumPy
- Pandas
- SciPy
- Scikit-learn
- LightGBM
- Google Colab / Jupyter Notebook

## Repository Contents

- `centroid_analysis_and_model_evaluation.ipynb` – Centroid feature extraction and model evaluation notebook.
- `README.md` – Project documentation.
- `.gitignore` – Files excluded from version control.

## Dataset Requirements

The pipeline expects the following input files:

- `train_centroid.npy`
- `test_centroid.npy`
- `train_stars.csv`
- `test_stars.csv`

These datasets are not included in this repository.

## Learning Outcomes

Through this hackathon, I explored:

- Feature engineering for time-series data.
- Statistical analysis of spatial measurements.
- Memory-efficient processing of large datasets.
- Multiclass machine learning.
- Cross-validation and model evaluation techniques.

## Note

This repository documents the Round 1 notebook and its implementation. The notebook's recorded execution encountered a missing input-data error, so no successful final evaluation score is claimed here.

---

**Event:** Hack4Hack 2026  
**Challenge:** Planet Hunters  
**Focus Area:** Centroid Analysis & Model Evaluation
