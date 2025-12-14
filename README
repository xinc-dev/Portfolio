# Public Transport Demand Forecasting

## Note on Data & Scope
This project mirrors a real-world public transport demand forecasting system developed in an industry setting. Due to data confidentiality, a publicly available dataset is used as a proxy. The production system operates on different data sources and includes additional business-specific logic.

---

## Overview
This project forecasts daily public transport demand across bus and rail services using historical trip data. It focuses on time-series forecasting under structural regime changes (COVID disruption and recovery) and evaluates model performance at multiple aggregation levels, from individual service lines to system-wide demand.

---

## Key Highlights
- Strong seasonal naïve baseline used as a primary benchmark  
- Rolling, time-aware cross-validation to prevent data leakage  
- Regularized linear models outperform tree-based models during volatile periods  
- Aggregation significantly improves forecast accuracy at mode and system levels  
- Deployment-ready forecasting pipeline implemented  

---

## Data
Daily trip counts by service line and transportation mode spanning **2019–2025**.

---

## Modeling Approach
- **Baseline:** 7-day seasonal naïve forecast  
- **Models:** Ridge Regression, Gradient Boosting, XGBoost, LightGBM  
- **Evaluation Metric:** Mean Absolute Error (MAE)  

Models are evaluated using rolling validation windows to reflect real-world forecasting constraints.

---

## Results
- Ridge Regression performs best during volatile recovery periods (2021–2023)  
- Seasonal naïve baseline remains highly competitive in stable post-2023 demand regimes  
- Aggregated forecasts (weekly and total demand) demonstrate strong accuracy and stability  

These findings highlight trade-offs between robustness and short-term adaptability in demand forecasting.

---

## Repository Structure
- `demand_forecasting.ipynb`: End-to-end analysis and evaluation  
- `src/`: Feature engineering and deployment-style forecasting pipeline  

---

## Limitations
- No explicit holiday or event features  
- Structural breaks remain challenging for all models  
- Model performance varies by aggregation level and demand regime  

---

## Next Steps
- Incorporate holiday and special-event calendars  
- Explore hybrid approaches combining naïve baselines with ML models  
- Extend the pipeline for automated retraining and monitoring  
