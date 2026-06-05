# LSTM Hyperparameter Sensitivity Analysis for Temperature Forecasting

## Project Overview

This project investigates the impact of key LSTM hyperparameters on temperature forecasting performance using real-world climate time series data.

Rather than focusing solely on generating accurate forecasts, the primary objective was to analyze how different model configurations influence prediction quality and model behavior.

The project explores the sensitivity of Long Short-Term Memory (LSTM) networks to hyperparameter selection and evaluates their effectiveness in a univariate temperature forecasting task.

---

## Research Question

**How do different LSTM hyperparameters affect forecasting performance in temperature prediction?**

To answer this question, multiple experiments were conducted by systematically varying important LSTM hyperparameters and comparing the resulting forecasting accuracy.

---

## Dataset

The project uses the **Daily Climate Time Series Dataset**, publicly available on Kaggle:

https://www.kaggle.com/datasets/sumanthvrao/daily-climate-time-series-data

The original dataset contains several meteorological variables, including:

* Mean Temperature
* Humidity
* Wind Speed
* Atmospheric Pressure

For this study, only the **temperature variable** was selected and modeled as a univariate time series.

---

## Objectives

* Explore temperature time series behavior
* Build forecasting models using LSTM networks
* Investigate the influence of hyperparameter selection
* Compare forecasting performance across configurations
* Identify hyperparameter settings that improve predictive accuracy

---

## Hyperparameters Investigated

### Sequence Length

The number of historical observations provided as input to the model.

The study evaluates how different input window sizes affect the model's ability to capture temporal dependencies.

### Forecast Length

The number of future values predicted by the model.

Different forecasting horizons were analyzed to determine how prediction difficulty increases over time.

### Learning Rate

The learning rate controls how quickly the model updates its weights during training.

Multiple values were tested to analyze convergence speed and forecasting accuracy.

### LSTM Units

The number of memory cells in the LSTM layer.

Experiments were conducted to evaluate how model capacity affects forecasting performance.

---

## Methodology

### Data Preparation

* Temperature extraction
* Missing value inspection
* Data normalization
* Sliding window generation
* Train/Test split

### Model Development

A Long Short-Term Memory (LSTM) neural network was implemented using TensorFlow/Keras.

The model was trained multiple times while varying the selected hyperparameters.

### Experimental Evaluation

Each configuration was evaluated independently and compared using forecasting performance metrics.

---

## Evaluation Metrics

The forecasting models were evaluated using regression metrics, including:

* Mean Absolute Error (MAE)
* Mean Squared Error (MSE)
* Root Mean Squared Error (RMSE)
* R² Score

The objective was to identify the configurations that produced the most accurate forecasts while maintaining stable training behavior.

---

## Visualizations

The notebook includes:

* Temperature trend analysis
* Forecasting results
* Predicted vs Actual comparisons
* Training history visualizations
* Hyperparameter comparison plots
* Forecast performance evaluation

---

## Technologies Used

* Python
* TensorFlow
* Keras
* Pandas
* NumPy
* Matplotlib
* Scikit-Learn
* Jupyter Notebook

---

## Repository Structure

```text
.
├── lstm_temperature_forecasting.ipynb
└── README.md
```

---

## Key Findings

The experiments demonstrate that forecasting performance is highly sensitive to hyperparameter selection.

Changes in sequence length, forecast horizon, learning rate, and network size can significantly influence prediction accuracy, highlighting the importance of systematic hyperparameter tuning in time series forecasting tasks.

---

## Learning Outcomes

Through this project, the following topics were explored:

* Time Series Forecasting
* Deep Learning
* Recurrent Neural Networks
* Long Short-Term Memory (LSTM)
* Hyperparameter Tuning
* Forecast Evaluation
* Experimental Design
* Sequential Data Modeling

