# Multi-Step Air Quality Forecasting

[![Keras](https://img.shields.io/badge/Keras-FF0000?style=for-the-badge&logo=keras&logoColor=white)](https://keras.io/)

The "Multi-Step Air Quality Forecasting" project is designed to predict air quality levels using a systematic pipeline with four key components.

## Overview

- **Framework Used**: Keras
- **Components**:
  1. Data Preprocessing
  2. Time-Series Decomposition
  3. Temporal Feature Extraction
  4. Prediction Layer

## Components

### Data Preprocessing

This component involves preparing the raw air quality data for analysis. It includes data normalization and transforming the data into a sliding window format to ensure compatibility with subsequent pipeline steps.

### Time-Series Decomposition

Here, the time-series data is decomposed into trend and seasonality components. This decomposition aids in understanding underlying patterns and trends, facilitating more accurate forecasts.

### Temporal Feature Extraction

Two LSTMs are utilized - one for the seasonal component and another for the trend component. Alternatively, an LSTM auto-encoder network is employed for seasonal and trend components in other architectures.

### Prediction Layer

Extracted features and learned temporal dependencies are combined to predict air quality for future time steps. The prediction layer comprises a simple feed-forward neural network, which maps the features to predicted air quality values.

Integrating these components into a cohesive pipeline aims to develop accurate forecasts of air quality levels, enhancing decision-making and planning in areas affected by air pollution.

## Environments

To set up the required environments, use the following commands:

```bash
pip install -U pip
pip install -r requirements.txt
```
