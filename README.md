Project: Exoplanet Detection – NACA Hackathon

Goal:
Detect confirmed exoplanets using Kepler datasets with a robust ML model.

Dataset Details:

Dataset used:
Evaluated 3 datasets; Dataset 3 was selected after addressing class imbalance and other issues.
Number of samples: 5979 (after cleaning)
Number of features: 116 (after cleaning)

Data Challenges:
Severe class imbalance
Overfitting risk
Missing values in some features
Pipeline in the Notebook:
Data Preprocessing
Handle missing values (numerical & categorical)
Label encoding for categorical features
Resampling
SMOTE used to balance classes

Model
LightGBM classifier with hyperparameter tuning
Early stopping on validation set

Evaluation
Train Accuracy: 98%
Test Accuracy: 95%
Confusion matrix & classification report included

Results Saved in Notebook:
Trained LightGBM model
Label encoder for target variable
Preprocessing objects (imputers, encoders, feature columns)

Saved Files (8 total):

File	Description
exoplanet_model.pkl	Trained LightGBM model
label_encoder.pkl	Target variable encoder
feature_columns.pkl	List of feature columns
feature_encoders.pkl	Encoders for categorical features
imputer_numeric.pkl	Imputer for numerical features
imputer_cat.pkl	Imputer for categorical features
numeric_columns.pkl	Names of numerical columns
cat_columns.pkl	Names of categorical columns

How to Use:
Download the repository (inference file + 8 model files) and install required libraries
Now u can use it and preprocess new data in Python.

Future Work (Ideas):
Extend model to other datasets

Experiment with deep learning approaches

Improve deployment pipeline or integrate into a web app
