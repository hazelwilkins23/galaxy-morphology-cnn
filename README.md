# Explainable AI for Galaxy Morphology Prediction

This project applies a Convolutional Neural Network (CNN) to classify galaxy morphologies using the Galaxy Zoo dataset. The goel is to predict morphological class probabilities and interpret the model's predictions using Explainable AI (XAI) techniques, specifically Saliency Maps. This project explores the effectiveness of deep learning models in astronomy and evaluates whether the model focuses on meaningful morphological features when making decisions.

## CONTENTS
ML_Project.ipynb – Main notebook for data aquisition, data preprocessing, model development, and evaluation.

Saliency_Maps.ipynb – Notebook for generating and visualizing saliency maps.

best_galaxy_hyperparams.txt – Final selected hyperparameters after tuning.

galaxy_prediction_results_final.csv – Prediction results and evaluation metrics.

requirements.txt – Project dependencies.

Final report (see report/ folder or attached PDF).

## DATASET
The dataset used in this project is from the Galaxy Zoo project. Galaxy images were retrieved using the SDSS SkyServer API based on object IDs provided in the Galaxy Zoo catalog. Due to size limitations and dataset restrictions, raw data is not included in this repository. Instructions for accessing the data can be found at Galaxy Zoo and the SDSS SkyServer.

## PROJECT OVERVIEW
A CNN model was trained to predict four morphological probabilities:
  - Edge-on Galaxy (P_EDGE)
  - Merger (P_MG)
  - Debiased Elliptical (P_EL_DEBIASED)
  - Debiased Combined Spiral (P_CS_DEBIASED)

The model achieved a final accuracy of 86% with a validation loss of 0.018 and a mean absolute error (MAE) of 0.092.

Saliency maps were generated to analyze which image regions influenced model predictions, providing insight into model interpretability and alignment with human classification heuristics.

## Dependencies
Install required libraries using the following command:

pip install -r requirements.txt

## RESULTS
The final CNN model demonstrated strong predictive performance, accurately classifying spiral and merger galaxies. The model struggled with elliptical and edge-on galaxies, particularly in noisy and dense cluster environments. Saliency map analysis confirmed that the model focused on key morphological features but had limitations when handling ambiguous images.

### Contact
Hazel Wilkins
hw30@fordham.edu
