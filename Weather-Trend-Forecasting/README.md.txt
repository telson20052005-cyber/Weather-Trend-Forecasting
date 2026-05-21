# Global Weather Trend Forecasting

## Project Overview

This project analyzes global weather data using advanced data science and machine learning techniques to forecast temperature trends and uncover environmental insights.

The project includes:
- Data cleaning and preprocessing
- Exploratory Data Analysis (EDA)
- Environmental impact analysis
- Spatial climate analysis
- Weather anomaly detection
- Multiple forecasting models
- Ensemble learning
- Advanced temporal feature engineering

The final forecasting system achieved strong predictive performance with an R² score of approximately **0.89** using an engineered ensemble model.

---

# PM Accelerator Mission

PM Accelerator aims to empower aspiring professionals through hands-on, industry-relevant AI, data science, and product management experiences by bridging the gap between academic learning and real-world applications.

---

# Dataset

Dataset used:

World Weather Repository Dataset from Kaggle:

:contentReference[oaicite:0]{index=0}

The dataset contains:
- Global weather observations
- Air quality metrics
- Atmospheric conditions
- Geographical information
- Temporal weather data

Total observations analyzed:
- ~4,000+ weather records
- 185 countries
- 41 original features

---

# Project Objectives

The main objectives of this project were:

- Analyze global weather patterns
- Perform environmental and spatial analysis
- Detect anomalous weather events
- Forecast temperature trends using machine learning
- Compare multiple forecasting algorithms
- Improve forecasting accuracy using feature engineering and ensemble learning

---

# Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- XGBoost
- LightGBM
- Jupyter Notebook

---

# Project Structure

```text
Weather-Trend-Forecasting/
│
├── data/
│   └── GlobalWeatherRepository.csv
│
├── notebooks/
│   └── Global_Weather_Trend_Forecasting.ipynb
│
├── images/
│
├── requirements.txt
├── README.md
```

---

# Data Preprocessing

The preprocessing pipeline included:

- Datetime conversion and validation
- Removal of malformed timestamps
- Missing value handling
- Redundant feature elimination
- Feature sanitization
- Temporal feature extraction
- Rolling statistical feature engineering

Redundant unit-based columns such as:
- Fahrenheit temperatures
- miles-based measurements
- duplicate wind metrics

were removed to reduce multicollinearity and improve model interpretability.

---

# Exploratory Data Analysis (EDA)

EDA techniques included:

- Temperature distribution analysis
- Correlation heatmaps
- Global precipitation trends
- Dual-axis climate visualizations
- Environmental correlation analysis
- Regional climate variability analysis

Key findings:
- Global temperatures were concentrated around 20°C–30°C
- UV Index strongly influenced temperature
- Humidity showed negative correlation with ozone concentration
- Significant spatial climate variability existed across countries

---

# Environmental Impact Analysis

The project analyzed relationships between:
- Weather conditions
- Air pollution metrics
- Atmospheric variables

Strong relationships were identified between:
- PM2.5
- PM10
- Ozone
- Nitrogen dioxide
- Weather parameters

This demonstrated the environmental influence of atmospheric pollutants on weather systems.

---

# Anomaly Detection

Advanced anomaly detection was performed using:
- Isolation Forest

Weather anomalies were identified using:
- Temperature
- Wind speed
- Atmospheric pressure
- Precipitation

Detected anomalies exhibited:
- Higher precipitation
- Stronger wind speeds
- Lower temperatures

indicating storm-like weather conditions.

---

# Spatial Climate Analysis

Spatial analysis was performed across the most statistically represented countries.

Key insights:
- Sudan exhibited the highest temperature profile
- Bolivia showed the highest climate variability
- Temperate regions demonstrated more stable weather distributions

---

# Machine Learning Models

The following forecasting models were implemented:

1. Linear Regression
2. Random Forest Regressor
3. Gradient Boosting Regressor
4. Voting Ensemble Regressor
5. Engineered Mega Ensemble
   - Random Forest
   - XGBoost
   - LightGBM

---

# Feature Engineering

Advanced temporal feature engineering included:

- Lag temperature variables
- Rolling humidity averages
- Rolling pressure averages
- Hour-of-day extraction
- Day-of-week extraction

Feature engineering significantly improved forecasting performance.

---

# Model Performance

| Model | MAE | RMSE | R² Score |
|---|---|---|---|
| Linear Regression | 4.10 | 5.10 | 0.51 |
| Random Forest | 2.39 | 3.35 | 0.78 |
| Gradient Boosting | 2.54 | 3.43 | 0.77 |
| Voting Ensemble | 2.39 | 3.29 | 0.79 |
| Engineered Mega Ensemble | 1.52 | 2.10 | 0.89 |

---

# Key Insights

- UV Index was the strongest predictor of temperature
- Feature engineering dramatically improved forecasting performance
- Ensemble learning improved prediction stability
- Weather anomalies were associated with high precipitation and wind conditions
- Spatial climate variability was significant across regions

---

# How to Run the Project

## 1. Clone the repository

```bash
git clone <your-github-repo-link>
```

## 2. Install dependencies

```bash
pip install -r requirements.txt
```

## 3. Open the notebook

```bash
jupyter notebook
```

Then open:

```text
Global_Weather_Trend_Forecasting.ipynb
```

---

# Future Improvements

Potential future enhancements include:

- Longer historical time-series forecasting
- Deep learning models (LSTM/Transformers)
- Real-time weather API integration
- Interactive dashboards using Streamlit
- Seasonal climate modeling
- Geospatial mapping visualizations

---

# Author

Telson Lalichen  
First Year Engineering Student  
Indian Institute of Technology Roorkee (IIT Roorkee)

---