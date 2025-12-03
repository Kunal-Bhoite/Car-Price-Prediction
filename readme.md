Car Price Prediction using Regularized Linear Models, SVR, and Random Forest

This project implements and compares multiple machine-learning regression techniques—including Regularized Linear Regression (L1, L2, Elastic Net), Support Vector Regression (SVR), and Random Forest Regression—to predict car prices using a structured automobile dataset.

The goal is to evaluate performance, interpretability, and the effect of different regularization strategies.

📁 Project Structure
├── ML_Dataset.csv                   # Dataset used for training & evaluation
├── Report_Car Price Prediction.py   # Full model training + comparison code
└── Report_Car Price Prediction.pdf # Project documentation/report

🚀 Features

Data pre-processing and category encoding (Target Encoding, label mapping)

Correlation analysis with annotated heatmap

Training & hyperparameter tuning using GridSearchCV

Implementation of:

L1 (Lasso) Regularization

L2 (Ridge) Regularization

Elastic Net Regularization

Support Vector Regression (SVR)

Random Forest Regression

Feature importance extraction (Random Forest)

Model comparison using R² and Modified R²

🛠️ Technologies Used

Python

Pandas

Scikit-Learn

Category Encoders

Plotly

NumPy



Install required dependencies:

pip install -r requirements.txt


If you don’t have a requirements.txt yet, the main packages are:

pandas
numpy
scikit-learn
plotly
category_encoders

📊 Dataset Overview

The dataset contains car attributes including:

brand

model

transmission

fuelType

mileage

year

tax

mpg

engineSize

price (target)

Categorical variables are encoded using Target Encoding and label mapping.

🔧 How to Run the Project

Run the Python file:

python Report_Car Price Prediction.py


This will:

Load & preprocess the dataset

Train regularized linear models

Train SVR and Random Forest

Perform GridSearchCV hyperparameter tuning

Output best parameters, R² score, modified R² score

Display correlation heatmap

List most important features (from RF)

📈 Model Performance Summary

Based on your report:

Model	                    Best R² Score	        Notes
Random Forest Regression	        95.31%	    Best performer overall
Support Vector Regression (SVR)	    87.57%	    Best with RBF kernel and C=10,000
Regularized Linear Regression	    76.68%	    Best with Elastic Net (L1 ratio = 1)

Conclusion:
👉 The dataset is non-linear in nature.
👉 Random Forest captures complex interactions best and gives the highest accuracy.

📘 Report

For detailed explanations of:

L1, L2, Elastic Net mathematical formulation

Interpretability comparison

SVR regularization effects

Random Forest performance interpretation

Refer to the included PDF report:
Report_Car Price Prediction.pdf



