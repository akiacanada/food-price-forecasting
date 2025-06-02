# 🌍 Food Price Forecasting Project

This project aims to build robust forecasting models for food prices across various countries using data provided by the World Food Programme (WFP). We explore different machine learning models — Prophet, XGBoost, and LSTM — to analyze seasonal trends, price fluctuations, and potential challenges in forecasting.

---

## Business Problem

Food price volatility poses significant risks to both consumers and policymakers, especially in developing countries. The goal of this project is to:

- Forecast monthly food prices using different modeling approaches.
- Provide insights for better resource allocation and policy formulation.
- Support humanitarian aid organizations and governments in preparing for price surges or shortages.

---

## Data Explanation

We use three key datasets:

- 'wfp_market_food_prices.csv': Raw food price data from various countries and markets.
- 'WLD_RTP_details_2023-10-02.csv': Metadata and additional details about food types and measurement units.
- 'WLD_RTFP_country_2023-10-02.csv': Country-level metadata for aggregation and filtering.

Key columns:
- 'adm0_name': Country name
- 'mp_month', 'mp_year': Month and year of price observation
- 'mp_price': Price of the commodity in local currency

---

## Methods

- **Prophet**: Time-series forecasting with trend and seasonality decomposition.
- **XGBoost**: Tree-based regression with feature engineering (month, year, lagged prices).
- **LSTM**: Deep learning approach capturing sequential dependencies in price trends.

---

## Results and Analysis

Visualizations and key metrics are included in:
- 'images/': Contains model forecasts for selected countries.
- 'reports/Food_Price_Forecasting_White_Paper.pdf': Includes an in-depth analysis of model performances, RMSE, and MAPE values.

Example visuals:
- Prophet forecast for India and Bangladesh
- XGBoost forecast for India
- LSTM forecasts for multiple countries

---

## Key Findings

- Prophet performed best for stable seasonal trends.
- XGBoost captured non-linear relationships in certain markets.
- LSTM showed promise but required more tuning due to data sparsity.

---

## Dependencies
pandas
numpy
matplotlib
seaborn
prophet
xgboost
tensorflow
scikit-learn

---

## How to Run

1. Clone the repository:
   '''bash
   git clone https://github.com/yourusername/food-price-forecasting.git
   cd food-price-forecasting

2. Install dependencies:
  pip install -r requirements.txt

3. Open the Jupyter Notebook in notebooks/ to explore the models.


## License
This project is shared for educational purposes.
