# real-estate-price-prediction
Predicting Georgia housing prices using EDA, Linear Regression, K-Means, and Random Forest

# Real Estate Price Prediction: Georgia Housing Market

A machine learning project that analyzes and predicts housing prices in the state of Georgia using real-world property data. The project includes extensive EDA, segmentation via K-Means clustering, and price prediction using linear and ensemble models.

---

## Project Goals

- **Predict** housing prices based on features like living area, bathrooms, bedrooms, and location.
- **Segment** the real estate market using clustering to identify patterns in property types.
- **Analyze** feature importance to determine which variables influence price the most.

---

## Tools & Libraries

- **Language:** R  
- **Visualization:** `ggplot2`, `plotly`, `corrplot`  
- **Modeling:** `randomForest`, `caret`, `stats`  
- **Data manipulation:** `dplyr`, `tidyr`, `lubridate`

---

## Exploratory Data Analysis (EDA)

- **Right-skewed distributions** for price and area → log-transformed
- Strong **positive correlation** between living area and price
- City-level variation observed (e.g., Atlanta, Marietta higher-priced)
- Correlation heatmaps revealed multicollinearity (e.g., between bedrooms and bathrooms)

---

## Models Used

| Model              | R² Score | RMSE         | Notes                                           |
|-------------------|----------|--------------|-------------------------------------------------|
| Linear Regression | 0.5745   | ~$307,991    | Interpretable baseline; underfits complex data  |
| Random Forest     | 0.8516   | ~$219,153    | Best performance; handles non-linearity well    |
| K-Means Clustering| —        | —            | Used for market segmentation, not prediction    |

---

## Highlights

- Identified **4 distinct property clusters** (e.g., luxury homes, starter homes)
- Found **living area, bathrooms, year built** to be most predictive
- Residual analysis confirmed low bias in Random Forest model

---

## Files

- `SLPROJECT.Rmd` – R Markdown file containing full analysis, models, and plots

---

## Future Improvements

- Incorporate **NLP** on property descriptions for richer features  
- Add **geospatial models** using coordinates or maps  
- Extend to include **temporal trends** or pricing over time

---
