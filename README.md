# Stock Market Prediction Using Machine Learning

This project builds a stock market prediction model using historical stock data, technical indicators, and a machine learning algorithm. The model uses free data obtained with [yfinance](https://github.com/ranaroussi/yfinance) and computes technical indicators such as SMA, EMA, and RSI with the [ta](https://github.com/bukosabino/ta) library. A Random Forest model from scikit-learn is trained to predict the next day’s closing price.

## Features

- **Data Collection:** Downloads historical stock data via yfinance.
- **Technical Indicators:** Computes Simple Moving Average (SMA), Exponential Moving Average (EMA), and Relative Strength Index (RSI).
- **Machine Learning:** Utilizes a Random Forest Regressor to predict future stock prices.
- **Visualization:** Uses Matplotlib and Plotly for interactive data visualization.
- **Reproducible:** All dependencies are listed in `requirements.txt` for easy setup.

## Project Structure

```
stock-market-prediction/
│
├── Stock_Price_Prediction.ipynb   # Main Jupyter Notebook with code and documentation.
├── requirements.txt               # List of Python packages and versions.
├── README.md                      # This README file.
└── .gitignore                     # Git ignore file to exclude unnecessary files.
```

## Setup Instructions

1. **Clone the Repository**

   ```bash
   git clone https://github.com/YOUR_USERNAME/stock-market-prediction.git
   cd stock-market-prediction
   ```

2. **Create and Activate a Virtual Environment (Recommended)**

   Using Conda:
   ```bash
   conda create -n stockpred python=3.10 -y
   conda activate stockpred
   ```

   Or using venv:
   ```bash
   python -m venv venv
   source venv/bin/activate   # On Windows use: venv\Scripts\activate
   ```

3. **Install Dependencies**

   ```bash
   pip install -r requirements.txt
   ```

4. **Run the Notebook**

   Start Jupyter Notebook and open `Stock_Price_Prediction.ipynb`:

   ```bash
   jupyter notebook
   ```

5. **Follow the Notebook Instructions**

   Execute each cell in the notebook to download the stock data, compute technical indicators, train the machine learning model, and visualize predictions.

## How It Works

- **Data Downloading:** Historical stock data (e.g., AAPL) is downloaded using yfinance for a specified period (e.g., 6 months).
- **Indicator Calculation:** The notebook computes SMA, EMA, and RSI to enrich the feature set for the ML model.
- **Model Training:** The data is split into training and testing sets; a Random Forest Regressor is then trained to predict future closing prices.
- **Prediction and Evaluation:** The model's performance is evaluated using metrics like Mean Squared Error, and actual vs. predicted prices are visualized.

## License

This project is open-source and available under the [MIT License](LICENSE).

## Acknowledgments

- [yfinance](https://github.com/ranaroussi/yfinance) for easy access to stock data.
- [ta](https://github.com/bukosabino/ta) for computing technical indicators.
- [scikit-learn](https://scikit-learn.org/) for providing robust machine learning tools.
```