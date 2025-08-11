# PV Power Forecasting using Ensemble Learning

This project forecasts photovoltaic (PV) power generation using a combination of statistical, deep learning, and transformer-based models. Predictions from multiple models are combined using a simple mean ensemble to improve accuracy.

## 📌 Features
- **Multiple Models Implemented**:
  - ARIMA & Seasonal ARIMA (SARIMA)
  - Vector AutoRegression (VAR)
  - Long Short-Term Memory (LSTM) networks
  - Convolutional Neural Networks (CNN) for time series
  - Multi-Layer Perceptron (MLP)
  - Transformer models for sequence forecasting
- **Ensemble Learning** — combines outputs from multiple models for robust predictions.
- **Data Visualization** — publication-quality plots using `scienceplots`.
- **Model Saving** — trained models saved in `.h5` format.

## 📂 Dataset
The project uses PV power generation data from `PVGen.csv`:
- **Columns**: Time-stamped readings of PV generation.
- **Sampling**: Subset of the first 190,000 readings is used for training/testing.
- **Preprocessing**: Date extraction, train/test splitting, normalization.


## 🛠 Installation
Install dependencies:
```bash
pip install pandas numpy matplotlib seaborn scikit-learn tensorflow pmdarima scienceplots statsmodels
```

If running in **Google Colab**, upload the dataset and install missing packages:
```python
!pip install scienceplots pmdarima
```

## 🚀 Usage
1. Open `PV_Forecating_Using_Ensemble_Learning.ipynb`.
2. Run all cells in sequence:
   - Load and preprocess data
   - Train individual models
   - Generate forecasts
   - Evaluate and visualize results
3. Saved models will appear as `.h5` files.

## 📊 Evaluation
Models are compared using **Mean Squared Error (MSE)** on the test set.  
Example comparison:
- Simple Mean Ensemble
- CNN
- MLP
- ARIMA
- LSTM
- VAR
- Transformer

## 📈 Example Output
- **Line plots**: Actual vs. predicted PV generation.
- **Bar charts**: MSE scores for each model.
- **Saved Plots**: `.svg` format for high-quality publication-ready figures.

## 📜 License
This repository is licensed under the MIT License — see the [LICENSE](LICENSE) file for details.
