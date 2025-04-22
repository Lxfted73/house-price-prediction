# House Price Prediction

Predict house prices using Kaggle’s House Prices: Advanced Regression Techniques dataset.

## Dataset
- Source: [Kaggle House Prices](https://www.kaggle.com/competitions/house-prices-advanced-regression-techniques)
- Features: `GrLivArea`, `Neighborhood`, `TotalSF` (engineered), etc.
- Target: `SalePrice`

## Methodology
- Preprocessed data: Handled missing values, encoded categorical features, scaled numerical features.
- Engineered features: Created `TotalSF` (total square footage).
- Trained Linear Regression and XGBoost models, achieving [insert RMSE, e.g., ~35,000 for XGBoost].
- Visualized predicted vs. actual prices and feature importance.

## Results
- **Linear Regression**: MSE: [insert], RMSE: [insert], R²: [insert]
- **XGBoost**: MSE: [insert], RMSE: [insert], R²: [insert]
- **Key Features**: `TotalSF`, `GrLivArea`, `Neighborhood_StoneBr` (see `feature_importance.png`).
- **Metrics**: Full details in `model_metrics.txt`.

## Setup
```bash
conda create -n ml-python-3-11 python=3.11
conda activate ml-python-3-11
pip install pandas==2.2.3 scikit-learn==1.6.1 xgboost==2.1.1 matplotlib==3.10.0 seaborn==0.13.2
jupyter notebook