"Enhancement in Properties of Mortar with Modified Recycled Aggregate by Enzyme Induced Carbonate Precipitation"

This repository contains the machine learning (ML) models and dataset used in my MSc thesis: “Enhancement in Properties of Mortar with Modified Recycled Aggregate by Enzyme Induced Carbonate Precipitation (EICP)” and The primary goal of these models is to predict the reduction of water absorption in recycled aggrgatemodified by using EICP, based on experimental and augmented data.
     
Repository Structure 

The repository is organized into three main folders:
1. Original Neon-Augmented Dataset Models
   
    Contains ML models built on the original dataset and neon-augmented dataset.
   
    Algorithms used:

         Linear Regression (LR)
   
         Decision Tree Regressor
   
         Random Forest Regressor
   
         AdaBoost Regressor
   
3. Augmented Dataset Models
   
   Contains ML models trained on further augmented datasets to enhance performance and robustness.
5. Selected Models for Laboratory Data Comparison
   
    Contains the best-performing models selected for validation against laboratory data.
   
    Includes Linear Regression for baseline comparison.
   
    Focus: Evaluating how well the models can predict water absorption reduction in modified recycled aggregate.

Objective

To integrate ML approaches into material science research and demonstrate how data-driven methods can:

Predict water absorption reduction in EICP-modified recycled aggregate.

Compare predicted results with laboratory experiments.

Provide insights for sustainable construction material design.

Guide to using the Trained Random Forest Model for Predictions
This guide provides step-by-step instructions on how to use the trained Random Forest model to predict 'Water Absorption reduction (%)' using new data.

Prerequisites:

Python installed with the necessary libraries (pandas, scikit-learn, numpy).
Access to the trained Random Forest model object (https://github.com/teme16alem/Temesgen-Alemayehu-Kassie).

Steps:

1. Load the trained model:

Load the saved Random Forest model object into your Python environment.

2. Prepare your new data:

Ensure your new data is in a format that can be loaded into a pandas DataFrame.
The DataFrame must have the same column names as the features used during training (excluding the target variable 'Water Absorption reduction (%)'). The required columns are: 'Temprature(℃)', 'PH', 'CaCl₂ (mol/L)', 'Soaking Time (days)', 'Converted Enzyme Conc (g/L)', and 'Urea Conc (g/L)'.

3. Make predictions:

Use the loaded trained Random Forest model to make predictions.
4. Interpret the predictions:

The output of the prediction will be an array or list of predicted 'Water Absorption reduction (%)' values corresponding to each row in your new data.


