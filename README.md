# Tata Motors Stock Price Prediction Using LSTM & ARIMA

This repository contains a project focused on predicting the stock prices of Tata Motors using Long Short-Term Memory (LSTM) neural networks. By leveraging historical stock price data, the LSTM model aims to forecast future stock prices, assisting in making informed investment decisions.

## Table of Contents

- [Introduction](#introduction)
- [Dataset](#dataset)
- [Installation](#installation)
- [Usage](#usage)
- [Model Architecture](#model-architecture)
- [Results](#results)
- [Contributing](#contributing)
- [License](#license)

## Introduction

Predicting stock prices is a significant challenge due to the market's inherent volatility and the multitude of factors influencing price movements. Traditional statistical methods often fall short in capturing the complex patterns in time-series data. LSTM neural networks, a type of Recurrent Neural Network (RNN), are well-suited for this task as they can learn long-term dependencies and patterns in sequential data, making them effective for time-series forecasting.

## Dataset

The dataset used in this project comprises historical stock prices of Tata Motors, including daily Open, High, Low, and Close prices, along with trading volume. The data spans from May 17, 2006, to October 11, 2021. You can download the dataset from Kaggle using the following link:

[https://www.kaggle.com/datasets/anoopjohny/tata-motors-stock-history](https://www.kaggle.com/datasets/anoopjohny/tata-motors-stock-history)

## Installation

To set up the project environment, follow these steps:

1. **Clone the repository:**

   ```bash
   git clone https://github.com/yourusername/tata-motors-stock-prediction.git
   cd tata-motors-stock-prediction
   ```

2. **Create and activate a virtual environment (optional but recommended):**

   ```bash
   python3 -m venv env
   source env/bin/activate  # On Windows, use 'env\Scripts\activate'
   ```

3. **Install the required dependencies:**

   ```bash
   pip install -r requirements.txt
   ```

## Usage

1. **Download the dataset:**

   Ensure you have downloaded the Tata Motors stock history dataset from the link provided above and place it in the `data/` directory of the project.

2. **Run the Jupyter Notebook:**

   Launch Jupyter Notebook and open the `tata_motors_stock_prediction.ipynb` file. This notebook contains the step-by-step process of data preprocessing, model building, training, and evaluation.

3. **Execute the notebook cells:**

   Follow the instructions within the notebook to preprocess the data, train the LSTM model, and visualize the predictions.

## Model Architecture

The LSTM model used in this project consists of the following layers:

- **LSTM Layer:** Captures temporal dependencies in the data.
- **Dropout Layer:** Prevents overfitting by randomly setting a fraction of input units to 0 during training.
- **Dense Layer:** Produces the final output.

The model is compiled using the Mean Squared Error (MSE) loss function and the Adam optimizer.

## Results

After training, the model's performance is evaluated using metrics such as Mean Absolute Error (MAE) and Root Mean Squared Error (RMSE). The notebook provides visualizations comparing the actual and predicted stock prices, demonstrating the model's ability to capture the general trend of Tata Motors' stock price movements.

## Contributing

Contributions to this project are welcome. If you have suggestions for improvements or new features, feel free to open an issue or submit a pull request.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for more details.

---

*Disclaimer: Stock price prediction is inherently uncertain and should not be used as financial advice. Invest responsibly.* 
