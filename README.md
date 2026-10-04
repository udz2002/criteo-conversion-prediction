# From Impressions to Conversions

## Predictive Modelling for Display Advertising Performance

This MSc Data Science project investigates whether machine-learning models can predict whether a digital display advertising impression will be followed by a conversion.

## Research Question

To what extent can machine-learning models predict whether a digital display advertising impression will be followed by a conversion, and which modelling approach provides the best performance for this highly imbalanced classification problem?

## Dataset

The project uses the Criteo Attribution Modeling for Bidding Dataset.

Dataset source:
https://www.kaggle.com/datasets/sharatsachin/criteo-attribution-modeling

The complete dataset contains 16,468,027 advertising impressions.

A reproducible 5% sample containing 823,401 impressions was used for model development because of computational constraints.

## Models Compared

- Logistic Regression
- Decision Tree
- Random Forest
- XGBoost
- Neural Network

## Evaluation Metrics

The models were evaluated using:

- Precision
- Recall
- F1-score
- ROC-AUC
- PR-AUC
- Log Loss
- Brier Score
- Conversion Lift

## Main Results

XGBoost achieved the strongest overall test performance:

- PR-AUC: 0.3121
- ROC-AUC: 0.8517
- F1-score: 0.3689

The top 10% of impressions ranked by XGBoost achieved approximately 5.27 times the conversion rate expected from random selection.

A separate experiment adding post-impression click information increased PR-AUC to 0.5300. Click was excluded from the primary impression-time model because it occurs after the impression has been served.

## Repository Structure

- `notebooks/` - project notebooks
- `scripts/` - reusable Python scripts
- `outputs/figures/` - visual outputs
- `outputs/tables/` - model and analysis results
- `data/` - dataset documentation
- `docs/` - supporting project documentation

## Reproducibility

A fixed random seed of 42 was used throughout the project where supported.

The dataset can be downloaded programmatically using KaggleHub.

## Author

Udara Withana  
MSc Data Science
