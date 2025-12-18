# Delhi Air Quality Forecasting

A comprehensive time series analysis and forecasting project for predicting PM2.5 concentrations in Delhi using statistical and deep learning models.

## Project Overview

This project aims to **forecast future air quality levels in Delhi**, specifically focusing on PM2.5 (Particulate Matter 2.5), by analyzing historical time series data from 2018-2023. Multiple modeling approaches are compared to determine which delivers the best predictive performance.

## Objectives

### Main Goal
Develop and compare various time series forecasting models to accurately predict PM2.5 concentrations in Delhi.

### Sub-Objectives

**Data Characterization:**
- Exploratory Data Analysis (EDA)
- Descriptive statistics
- Time series visualization
- Stationarity checks
- Seasonal decomposition

**Model Development:**
- **Statistical Models**: ARIMA, SARIMA, Decomposition-based forecasting
- **Neural Network Models**: RNNs, LSTMs, CNNs, MLP-based models
- Hyperparameter tuning and optimization

## Key Research Questions

1. How accurately can we forecast PM 2.5 concentrations in Delhi, and which time-series models deliver the best predictive performance?
2. What strength and periodicity of trend/seasonality exist in relevant pollutants and meteorological features?

## Dataset

### Source
Data downloaded from [Kaggle: Time Series Air Quality Data of India (2010-2023)](https://www.kaggle.com/datasets/abhisheksjha/time-series-air-quality-data-of-india-2010-2023/)

### Delhi Dataset (DL019.csv)
- **Time Period**: February 1, 2018 - March 31, 2023
- **Total Records**: 45,230 (approximately 5 years of hourly data)
- **Data Quality**: Least missing values among available regions
- **Source**: Central Control Room for Air Quality Management

### Pollutants Measured
- PM2.5, PM10 (ug/m³)
- NO, NO₂, NOₓ, NH₃, SO₂, CO (various units)
- Ozone (ug/m³)
- Benzene, Toluene (ug/m³)

### Meteorological Features
- Temperature (°C)
- Relative Humidity (%)
- Wind Speed (m/s) & Direction (°)
- Solar Radiation (W/m²)
- Barometric Pressure (mmHg)
- Rainfall (mm)

## Files

- `delhi_project_MyatMaDeMayPhuuNgon.ipynb` - Main analysis and forecasting notebook
- `DL019.csv` - Delhi air quality dataset

## Technologies & Libraries

- **Data Processing**: Pandas, NumPy
- **Visualization**: Matplotlib, Seaborn
- **Statistical Modeling**: Statsmodels (ARIMA, SARIMA)
- **Deep Learning**: TensorFlow, Keras
- **Evaluation**: Scikit-learn metrics

## Project Structure

The Jupyter notebook is organized into the following sections:

1. **Data Loading & Exploration** - Initial dataset overview and statistics
2. **Data Preprocessing** - Cleaning, handling missing values, feature engineering
3. **Time Series Analysis** - Decomposition, stationarity tests, autocorrelation
4. **Statistical Models** - ARIMA/SARIMA implementation and evaluation
5. **Neural Network Models** - LSTM, CNN, and other deep learning approaches
6. **Model Comparison** - Performance metrics and comparative analysis
7. **Forecasting Results** - Future predictions and visualizations
8. **Conclusions** - Key findings and recommendations

## Usage

1. Clone the repository:
   ```bash
   git clone https://github.com/Myatmade/DelhiAirQuality_Forecast.git
   cd DelhiAirQuality_Forecast
   ```

2. Install required dependencies:
   ```bash
   pip install pandas matplotlib seaborn numpy scikit-learn statsmodels tensorflow keras
   ```

3. Open the Jupyter notebook:
   ```bash
   jupyter notebook delhi_project_MyatMaDeMayPhuuNgon.ipynb
   ```

4. Run the cells sequentially to reproduce the analysis and forecasting results.

## Results & Findings

The notebook contains detailed analysis including:
- Seasonal patterns and trend analysis of PM2.5
- Comparative performance metrics for all models
- Visual representations of forecasts vs actual values
- Statistical significance tests
- Recommendations for best-performing models

## Author

**Myat Ma De May Phuu Ngon**

**Course**: Applied Informatics 1 - 2025 ISSE Third Year Spring Semester

## License

This project is licensed under the MIT License - see the LICENSE file for details.

## References

- Kaggle Dataset: Time Series Air Quality Data of India
- Central Control Room for Air Quality Management, India
- Time Series Analysis and Forecasting literature
