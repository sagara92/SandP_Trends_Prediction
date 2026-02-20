# S&P 500 Trends Prediction

## Project Overview
In this project I aim to predict the trends of the S&P 500 index using various probabilistic and machine learning models. The core implementation involves a **Hidden Markov Model (HMM)** to forecast future prices based on hidden market states, and other models include **ARIMA** and **LSTM** (to be implemented) and I compare the performance of these models for time-series forecasting.

## Functionality
The python script and Jupyter Notebook perform the following steps:
1.  **Data Acquisition**: Downloads S&P 500 historical data from Kaggle (`sp500_index.csv`). If the data already exists locally, the download is skipped.
2.  **Data Preprocessing**: Loads and cleans the data for modeling.
3.  **HMM Implementation**: Uses a Gaussian HMM to model latent states of the market and predict future price movements.
4.  **Visualization**: Generates plots for forecasts, including uncertainty intervals and residuals.
5.  **ARIMA Implementation**: Implements an AutoRegressive Integrated Moving Average model to capture trend and noise, to be implemented.

## Models and Performance

### Hidden Markov Model (HMM)
The HMM model assumes the market transitions between hidden states (e.g., bull, bear, stagnant) and outputs observed prices.
-   **Directional Accuracy**: The HMM model achieved a directional accuracy of **72.73%** in predicting price movements over a window of 22 trading days.
-   **Forecast Plot**: The notebook outputs a visualization of the **S&P 500 HMM Forecast**, which includes a **$1\sigma$ Uncertainty** representing the confidence interval of the predictions and **Residuals** plot to visualize the prediction error over time.

## Dependencies
-   `numpy`
-   `pandas`
-   `matplotlib`
-   `hmmlearn`
-   `statsmodels`
-   `kaggle`
