This project explores and forecasts **global temperature anomalies** using historical climate data. It leverages machine learning (Gradient Boosting) and time series forecasting (Prophet) to model and predict climate change trends based on key indicators such as CO₂ emissions, sea surface temperature (SST), and sea level rise.

---

## Project Overview

- Analyze and preprocess global datasets: temperature anomalies, CO₂ emissions, sea levels, and sea surface temperature.
- Train a **Gradient Boosting Regressor** to predict temperature anomalies.
- Evaluate model performance (R², RMSE, MAE).
- Use **Prophet** for long-term time series forecasting of global temperature anomalies.

---

## Datasets Used

| Dataset | Description | Source |
|--------|-------------|--------|
| Monthly Global Temperature | Global land/ocean temp anomalies | [GitHub Dataset](https://github.com/datasets/global-temp) |
| CO₂ Emissions | Fossil fuel CO₂ emissions by year | [GitHub Dataset](https://github.com/datasets/co2-fossil-global) |
| Sea Level Rise | Global sea level trend | [DataHub](https://datahub.io/core/sea-level-rise) |
| SST Data | NOAA Annual Land-Ocean Temp | [NOAA](https://www.ncei.noaa.gov/) |

---

## Technologies Used

- Python
- Pandas, NumPy
- Scikit-learn
- Prophet
- Matplotlib, Seaborn

---

## Model Training

**Gradient Boosting Regressor:**

- Features:
  - Year, Year²
  - CO₂ Emissions (lag, delta)
  - SST (lag, delta, rolling mean)
- Evaluation:
  - R² Score: **0.927**
  - RMSE: **0.085**
  - MAE: **0.067**
