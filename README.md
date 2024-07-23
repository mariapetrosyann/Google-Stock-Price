# Google Stock Price Prediction

This repository contains a machine learning project designed to predict Google's stock prices using historical data. The project utilizes Long Short-Term Memory (LSTM) networks to forecast future stock prices based on past performance.

## Table of Contents

- [Project Overview](#project-overview)
- [Features](#features)
- [Setup](#setup)
- [Usage](#usage)
- [Model Architecture](#model-architecture)
- [Results](#results)
- [Contributing](#contributing)
- [License](#license)

## Project Overview

The aim of this project is to build a predictive model for Google's stock prices using historical data. The model employs LSTM networks, a type of Recurrent Neural Network (RNN) well-suited for time series forecasting. This project is intended to predict future stock prices by learning from past trends and patterns.

## Features

- **Data Preprocessing:** Normalization and preparation of time series data suitable for LSTM input.
- **Model Building:** An LSTM-based neural network architecture for accurate stock price prediction.
- **Evaluation:** Performance metrics including Mean Absolute Error (MAE) and Root Mean Squared Error (RMSE) to assess model accuracy.
- **Visualization:** (Optional) Visualization of predicted vs. actual stock prices (if implemented).

## Setup

To run this project, set up your environment and install the required dependencies.

### Prerequisites

- Python 3.x
- Google Colab or a similar environment (optional)
- Basic knowledge of machine learning and time series forecasting

### Installing Dependencies

Create a virtual environment and install the necessary packages:

```bash
pip install numpy pandas keras scikit-learn matplotlib
```

## Usage

Follow these steps to execute the project:

1. **Clone the Repository:**

   ```bash
   git clone https://github.com/yourusername/Google-Stock-Price.git
   cd Google_Stock_Price
   ```

2. **Prepare the Dataset:**

   Place your dataset file (e.g., `GOOG.csv`) in the project directory. The dataset should include historical stock price data, with at least a "Close" column.

3. **Run the Code:**

   Open the `Google_Stock_Price.ipynb` notebook (if using Google Colab) 
   

4. **Evaluate the Model:**

   The model will be trained and evaluated. The performance metrics, such as MAE and RMSE, will be displayed in the output.

## Model Architecture

The LSTM model used in this project is configured as follows:

- **First LSTM Layer:** 50 units, `return_sequences=True` to output the full sequence of the input.
- **Second LSTM Layer:** 50 units, `return_sequences=False` to output the final time step.
- **Dense Layer:** 25 units for feature transformation.
- **Output Dense Layer:** 1 unit to produce the final stock price prediction.

**Compile Configuration:**

- **Optimizer:** Adam.
- **Loss Function:** Mean Squared Error (MSE).

## Results

The model's performance metrics are:

- **Root Mean Squared Error (RMSE):** [55.967]

These metrics indicate how well the model's predictions align with the actual stock prices.

## Contributing

Contributions are welcome! If you have suggestions for improvements or fixes, please open an issue or submit a pull request.
