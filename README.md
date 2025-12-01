Hydrocarbon Heat Dynamic Predictions Using RDKit and Machine Learning
Overview

This project explores the use of RDKit in conjunction with machine learning to model the thermal properties of hydrocarbons. Hydrocarbons, composed solely of carbon and hydrogen, are essential fuels. Predicting their melting and boiling points helps understand their thermodynamic behavior.

Tools & Libraries

Python

Pandas, NumPy

Matplotlib, Seaborn

RDKit

Scikit-learn (Linear Regression, Polynomial Regression, Random Forest Regressor)

Dataset

Contains hydrocarbons with SMILES representation.

Features extracted: atomic weight and number of aromatic rings.

Targets: Melting point and Boiling point.

Project Tasks
1. Data Preprocessing

Installed RDKit for cheminformatics operations.

Loaded dataset and extracted molecular descriptors (atomic weight, aromatic rings).

Cleaned dataset by removing rows with missing target values.

2. Exploratory Analysis

Generated scatter plots for melting and boiling points vs molecular weight.

Observed positive correlation for boiling points; melting points were more scattered due to additional structural factors.

3. Model Training

Linear Regression: Established baseline; moderate accuracy for melting points, high accuracy for boiling points.

Polynomial Regression (Degree 3): Improved performance, capturing non-linear relationships; R² of 0.67 (melting) and 0.98 (boiling).

Random Forest Regression: Strong performance, especially for boiling points; able to model complex non-linear dependencies.

4. Model Evaluation

Evaluated models using Mean Squared Error (MSE) and R² scores.

Compared models in a summary table.

Visualized actual vs predicted values for all models, confirming improved fit for Polynomial and Random Forest regressions.

5. Challenges & Improvements

Limited feature set reduced melting point prediction accuracy.

Missing data decreased dataset size.

Future improvements: include additional RDKit descriptors, apply cross-validation, hyperparameter tuning, explore advanced models like Gradient Boosting.

Key Learnings

Non-linear models capture hydrocarbon thermal behavior better than linear regression.

Molecular descriptors such as atomic weight and aromatic rings are critical predictors.

Visualizations confirm model performance and highlight differences between melting and boiling point predictions.

How to Run

Clone the repository.

Install dependencies: pip install -r requirements.txt

Open the notebook hydrocarbon_heat_dynamics.ipynb in Jupyter or Google Colab.
