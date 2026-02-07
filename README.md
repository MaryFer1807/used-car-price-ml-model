# Used Car Price Prediction – Machine Learning Project

## Project Overview
This project focuses on building a machine learning system to predict the **market value of used cars**. The solution is designed for a real-world application where not only prediction quality matters, but also **training time** and **prediction speed**.

Multiple machine learning models are trained and compared to identify the best trade-off between accuracy and performance.

## Objective
The main goals of this project are to:
- Predict used car prices based on technical specifications and historical data.
- Compare different machine learning models in terms of:
  - Prediction quality (RMSE)
  - Training time
  - Prediction speed
- Identify the most suitable model for deployment in a production environment.

## Dataset
The dataset used:
- `car_data.csv`

Features include:
- Vehicle type, brand, model, fuel type
- Registration year and month
- Gearbox type
- Power
- Mileage
- Repair history
- Additional metadata related to listing activity

Target variable:
- `Price` (in euros)

## Data Preparation
- Removed irrelevant and non-informative features.
- Cleaned anomalous values (incorrect years, unrealistic power and mileage).
- Processed categorical variables using appropriate encoding techniques.
- Prepared consistent training and validation datasets.

## Modeling Approach
Several machine learning models were trained and evaluated:

- **Linear Regression**  
  Used as a baseline sanity check.

- **Decision Tree / Random Forest**  
  Tree-based models with hyperparameter tuning to improve performance.

- **Gradient Boosting Models**  
  Advanced boosting algorithms used to achieve higher accuracy:
  - LightGBM (with hyperparameter tuning)
  - CatBoost (optional)
  - XGBoost (optional)

Special attention was given to:
- Feature encoding differences between models
- Computational cost during training
- Prediction latency

## Evaluation Metric
Model performance was evaluated using:
- **RMSE (Root Mean Squared Error)**

Additional metrics:
- Training time
- Prediction time

These metrics were used to assess real-world deployment feasibility.

## Performance Analysis
- Compared model accuracy against training and inference speed.
- Verified that gradient boosting models outperform linear regression.
- Analyzed whether higher accuracy justifies longer training time.
- Selected the most balanced model for production use.

## Tools Used
- Python
- Pandas
- NumPy
- Scikit-learn
- LightGBM
- CatBoost (optional)
- XGBoost (optional)
- Matplotlib
- Jupyter Notebook

## Business Value
This project demonstrates the ability to:
- Build production-oriented machine learning models.
- Evaluate trade-offs between accuracy and performance.
- Work with large datasets and complex feature spaces.
- Select models suitable for real-time price estimation systems.

The approach is directly applicable to automotive platforms, marketplaces, and pricing intelligence systems.
