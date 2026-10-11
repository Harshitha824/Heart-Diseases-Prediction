# Heart Disease Prediction: Feature Selection, Stability and Generalisation

## About the Project

This research project investigates how feature-selection strategies influence the performance, stability, and cross-dataset generalisation of machine-learning models for heart-disease prediction.

Rather than focusing only on achieving high prediction accuracy, the study examines whether reducing the number of input features produces consistent benefits across different algorithms, evaluation metrics, and datasets.

The experiments are conducted using Python in Google Colab.

## Research Objectives

- Evaluate the effect of feature selection on predictive performance.
- Compare SelectKBest and Mutual Information feature-selection methods.
- Investigate how the number of selected features affects model performance.
- Examine feature-selection stability across cross-validation folds.
- Evaluate cross-dataset generalisation using Cleveland and Hungarian heart-disease datasets.
- Compare multiple evaluation metrics instead of relying on accuracy alone.

## Machine Learning Algorithms

The following algorithms are evaluated:

- Logistic Regression
- K-Nearest Neighbors (KNN)
- Support Vector Machine (SVM)
- Decision Tree
- Random Forest
- Naive Bayes

## Dataset

The study uses heart-disease data from the UCI Machine Learning Repository.

**Datasets:**
- Cleveland Heart Disease dataset
- Hungarian Heart Disease dataset

For cross-dataset comparisons, the experiments use ten common input features:

`age`, `sex`, `cp`, `trestbps`, `chol`, `fbs`, `restecg`, `thalach`, `exang`, and `oldpeak`.

Dataset source: [UCI Heart Disease Dataset](https://archive.ics.uci.edu/dataset/45/heart+disease)

## Methodology

The experimental workflow includes:

1. Dataset loading and preparation
2. Missing-value imputation and feature scaling
3. Baseline model evaluation
4. Feature selection using SelectKBest and Mutual Information
5. Evaluation of different feature counts
6. Feature-selection stability analysis
7. Five-fold and repeated five-fold cross-validation
8. Cross-dataset evaluation in both directions:
   - Cleveland → Hungarian
   - Hungarian → Cleveland
9. Comparative analysis of model performance and variability

Feature selection and preprocessing are incorporated into machine-learning pipelines where appropriate to reduce data leakage during cross-validation.

## Evaluation Metrics

Models are evaluated using:

- Accuracy
- Precision
- Recall
- F1-score
- ROC-AUC

Repeated cross-validation is also used to examine variation in model performance.

## Preliminary Findings

The experiments conducted so far indicate that:

- Feature selection does not consistently improve every model.
- Its effect varies with the algorithm and evaluation metric.
- Feature dimensionality influences predictive performance.
- Some features are selected consistently across validation folds.
- Stable feature subsets can preserve much of the predictive performance for some models, while reducing performance for others.
- Performance can change when models are transferred between datasets.

These are preliminary experimental observations and are not evidence of clinical effectiveness.

## Repository Contents

- `Heart_Disease.ipynb` — Jupyter notebook containing the research experiments, model evaluations, and analysis.

## Technologies Used

- Python
- Google Colab
- Pandas
- NumPy
- Scikit-learn
- Matplotlib
- Seaborn
- UCI Machine Learning Repository

## Current Status

**Research and experimental evaluation in progress.**

The current work focuses on understanding feature-selection stability and cross-dataset generalisation. The final research title, research gap, and conclusions will be finalized after the experimental findings and literature review are consolidated.

## Disclaimer

This project is for academic research and educational purposes only. The models are experimental and are not intended to diagnose heart disease or replace professional medical advice.

## Author

**Harshitha S.**

Computer Science and Engineering Student

GitHub: [Harshitha824](https://github.com/Harshitha824)
