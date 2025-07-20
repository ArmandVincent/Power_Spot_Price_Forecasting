# Power Spot Price Forecasting

This repository provides a complete workflow for forecasting electricity spot prices using machine learning and time series models. The project includes data exploration, feature engineering, regression/classification with CART and Random Forest, and time series forecasting with ARIMA and VAR.

## Project Structure

- `data/`  
  Contains raw and preprocessed datasets for training and testing.

- `output/`  
  Stores model predictions and forecast results.

- `src/`  
  Jupyter notebooks for each stage:
  - `01_data_exploration.ipynb`: Data loading, cleaning, feature engineering, and visualization.
  - `02_CART.ipynb`: CART regression and classification, grid search, evaluation.
  - `03_random_forest.ipynb`: Random Forest regression/classification, hyperparameter tuning, evaluation.
  - `04_times_series.ipynb`: Time series analysis and forecasting with ARIMA and VAR.

## Workflow

1. **Data Exploration**  
   - Inspect and clean the data.
   - Engineer time-based and holiday features.
   - Impute missing values using mean and KMeans clustering.

2. **CART & Random Forest Models**  
   - Train regression and classification models.
   - Perform grid search for hyperparameter optimization.
   - Display top 10 hyperparameter sets.
   - Evaluate models with appropriate metrics.

3. **Time Series Forecasting**  
   - Analyze stationarity and autocorrelation.
   - Fit ARIMA and VAR models for forecasting.
   - Visualize and export forecast results.

## Requirements

- Python 3.8+
- pandas, numpy, matplotlib, seaborn
- scikit-learn
- statsmodels
- holidays

Install dependencies with:

```bash
pip install pandas numpy matplotlib seaborn scikit-learn statsmodels holidays
```

## Usage

Open the notebooks in the `src/` folder and run each cell sequentially. Outputs and forecasts are saved in the `output/` directory.

## License

MIT License