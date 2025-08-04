# Sonalgaz_Stage
Forecasting monthly gas consumption for Ali Mendjeli and Constantine using ARIMA and Random Forest.
# Electricity and Gas Consumption Analysis

## Project Overview
This project analyzes electricity and gas consumption data for two regions, Ali Mendjli and Constantine, using a dataset from Sonalgaz. The analysis includes data exploration, visualization, and predictive modeling using ARIMA and Random Forest models to forecast electricity consumption. The dataset is processed and visualized using Python, with key libraries including Pandas, NumPy, Matplotlib, and Seaborn.

## Dataset
The dataset (`Consomation Sonalgaz.xlsx`) contains monthly electricity and gas consumption data from January 2006 to December 2023 for two regions. It includes the following columns:
- **Date**: The date of the observation (monthly, starting from 2006-01-01).
- **Region**: The region of consumption (Ali Mendjli or Constantine).
- **Consomation Elec**: Electricity consumption (in unspecified units).
- **Consomation gaz**: Gas consumption (in unspecified units).

Key dataset statistics:
- Total records: 432 (216 per region).
- Time span: January 2006 to December 2023.
- Electricity consumption: Mean = 30.31, Min = 12.33, Max = 65.73.
- Gas consumption: Mean = 163.68, Min = 17.01, Max = 530.83.

## Project Structure
The main analysis is performed in the Jupyter Notebook `Consomation elec.ipynb`. The notebook includes:
1. **Data Loading and Exploration**:
   - Loading the dataset using Pandas.
   - Basic exploration using `.head()`, `.shape`, `.describe()`, and `.value_counts()` to understand the data structure and summary statistics.
2. **Data Visualization**:
   - A plot comparing real electricity consumption values with predictions from ARIMA and Random Forest models for a selected region.
   - Visualization includes date-based trends with rotated x-axis labels for readability.
3. **Predictive Modeling**:
   - **ARIMA Model**: Used for time-series forecasting of electricity consumption. Performance metrics: RMSE = 6.53, R² = 0.58.
   - **Random Forest Model**: Used for predicting electricity consumption. Performance metrics: RMSE = 5.29, R² = 0.77.
   - Comparison of predictions against real values in a single plot, showing Random Forest outperforming ARIMA in both RMSE and R².

## Dependencies
To run the notebook, install the following Python libraries:
```bash
pip install pandas numpy matplotlib seaborn
