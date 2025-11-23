# Song Popularity Predictor
# 🎵 Spotify Song Popularity Predictor (XGBoost Regression)

## 🚀 Project Overview

This project develops a highly accurate Machine Learning model to predict the **popularity score (0-100)** of songs based solely on their objective audio features (acousticness, danceability, energy, etc.) and metadata.

The final model, a **Tuned XGBoost Regressor**, achieved excellent performance, demonstrating the strong correlation between objective musical characteristics and commercial success.

## 📊 Final Performance Metrics

| Metric | Result | Interpretation |
| :--- | :--- | :--- |
| **R-squared (R²)** | **0.7496** | The model explains approximately **75%** of the variance in song popularity. |
| **RMSE** | **10.98** | On average, predictions are off by only **10.98 points** on the 0-100 popularity scale. |
| **Best Model** | **XGBoost Regressor** | Final parameters were optimized via Randomized Search. |

## ✨ Key Technical Highlights

* **Feature Engineering:** Successfully created a robust **Song Recency** feature (days since release) to model popularity decay over time, which proved to be a critical predictor.
* **Data Strategy:** Implemented **Target Encoding** on the Artist feature to convert high-cardinality text data into a powerful numerical predictor, maximizing model signal while preventing data leakage.
* **Model Tuning:** Used **Randomized Search with Cross-Validation** to efficiently tune the XGBoost model's hyperparameters (e.g., `max_depth`, `n_estimators`) for peak performance.

## 📦 Repository Structure
- main.ipynb
- data.csv
- requirements.txt
- actual_vs_predicted_popularity.png
- feature_importance.png
