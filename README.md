# Driver Drowsiness Prediction using Physiological Signals

This project was completed during my **Erasmus+ exchange semester at Hochschule Trier (HS Trier), Germany**, as part of the **KiDA (Artificial Intelligence & Data Analytics)** course.

The goal of the project was to predict **driver drowsiness** from physiological signals using a **Regression Artificial Neural Network (ANN)**. The system estimates the **Karolinska Sleepiness Scale (KSS)** from features extracted from Photoplethysmography (PPG) signals, providing a non-invasive approach for monitoring driver fatigue.

---

## Project Overview

The complete machine learning pipeline consists of:

- Physiological signal acquisition using BITalino
- Signal preprocessing
- PPG feature extraction
- Regression Artificial Neural Network (ANN)
- Driver drowsiness prediction using KSS
- Evaluation using multiple validation strategies

The model was evaluated using three different validation approaches:

| Validation Strategy | MAE |
|--------------------|-----|
| Chunk Split | **0.74** |
| Session Split | **0.79** |
| Patient Split | **1.87** |

These experiments demonstrate how increasingly realistic validation strategies affect the model's generalization performance.

---

## My Contribution

This was a **team project** completed together with:

- Ayah Said
- Mohammad Al-Omaishat
- Bani Meshal

My primary responsibility focused on the **machine learning stage** of the project after feature extraction.

Specifically, I:

- Designed the Regression Artificial Neural Network (ANN)
- Implemented the complete TensorFlow/Keras regression model
- Performed hyperparameter optimization
- Evaluated the model using Chunk, Session, and Patient Split strategies
- Compared model performance using Mean Absolute Error (MAE)
- Analyzed and interpreted the experimental results
- Wrote the ANN, Results, Discussion, and Conclusion sections of the final IEEE report

---

## Repository Structure

- 📓 [Regression ANN Model](notebooks/regression_ann_model.ipynb)
- 📓 [PPG Preprocessing & Feature Extraction](notebooks/ppg_preprocessing_feature_extraction.ipynb)
- 📄 [Project Report](Driver_Drowsiness_Prediction_Report.pdf)

- **regression_ann_model.ipynb**  
  Regression ANN implementation, training, hyperparameter optimization, and evaluation.

- **ppg_preprocessing_feature_extraction.ipynb**  
  Signal preprocessing and extraction of physiological features from PPG recordings.

---

## Technologies Used

- Python
- TensorFlow / Keras
- NumPy
- Pandas
- Scikit-learn
- NeuroKit2
- Matplotlib
- Jupyter Notebook

---

## Results

The proposed ANN successfully predicts continuous Karolinska Sleepiness Scale (KSS) values from six physiological PPG features.

The experiments showed:

- Excellent performance on Chunk and Session Split validation.
- Patient Split remains the most challenging scenario because it evaluates completely unseen participants.
- Validation strategy has a major influence on measured model performance.

---

## Report

The complete IEEE-style project report is available here:

[📄 Driver_Drowsiness_Prediction_Report.pdf](Driver_Drowsiness_Prediction_Report.pdf)

---

## Acknowledgements

This project was completed during my **Erasmus+ exchange semester at Hochschule Trier (Germany)** as part of the **KiDA course** in collaboration with my teammates.
