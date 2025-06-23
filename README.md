
 🧠 Trader Behavior Insights

This project explores the relationship between market sentiment (Fear & Greed Index) and individual trader behavior using historical trading data. The analysis includes data cleaning, feature engineering, statistical testing, machine learning model training, and performance evaluation to generate actionable insights.

---

## 📁 Project Overview

This notebook investigates how extreme sentiment conditions influence trader performance and explores the potential of sentiment-driven features to predict future trading outcomes such as **Closed PnL**.

---

## ⚙️ Environment Setup

If using **Google Colab**, most dependencies are pre-installed.

To enable GitHub integration for notebook uploads:

1. Generate a **GitHub Personal Access Token** with the `repo` scope.
2. Store it in Colab as:

   * `github_token`: your personal access token
   * `github_username`: your GitHub username

These secrets can be added via the **Userdata** section in Colab.

---

## 🚀 Running the Notebook

To execute this project:

1. Upload the notebook `Trader Behavior Insights.py` to [Google Colab](https://colab.research.google.com/).
2. Upload the datasets:

   * `historical_data.csv`
   * `fear_greed_index.csv`
3. Run all cells sequentially from top to bottom.

The notebook will generate:

* Summary statistics
* Data visualizations
* Statistical test results (T-tests, ANOVA)
* Machine learning model outputs (metrics, feature importances)

---

## 📊 Key Findings and Conclusions

* **Sentiment Impact on Performance:** Significant differences in trader performance were observed under **Extreme Fear** and **Extreme Greed** conditions, with shifts in average PnL and trade behavior.
* **PnL Distribution:** Visual and statistical analysis revealed notable differences in PnL distributions across sentiment classifications.
* **Trade Size vs. PnL:** A potential correlation was observed between trade size (rolling average) and profit/loss outcomes.
* **Model Performance:** A **Random Forest Regressor** was trained to predict 'Closed PnL' based on engineered features. Results were evaluated using MSE, MAE, and R².
* **Optimization Gains:** Model performance improved following **hyperparameter tuning** using `GridSearchCV`.

---

## 🔧 Feature Engineering Highlights

* Lagged sentiment and PnL features (`1-day`, `2-day`, `3-day`)
* Rolling metrics:

  * 7-day rolling average PnL (`rolling_avg_pnl_7d`)
  * 3-day rolling sum PnL (`rolling_sum_pnl_3d`)
* Account-level cumulative PnL
* Trade size smoothing via 10-period rolling average

---

## 🔮 Future Work

This project opens up several avenues for expansion:

* 📈 **Enhanced Feature Set:** Integrate technical indicators (e.g., RSI, MACD), crypto market caps, or real-time news sentiment.
* 🧪 **Advanced Modeling:** Explore time series models (e.g., ARIMA, LSTM) for temporal prediction.
* 🔍 **Asset-Level Analysis:** Assess sentiment's impact across different tokens (`Coin`), and identify asset-specific behavior patterns.
* 🧭 **Strategy Evaluation:** Investigate optimal trading strategies under different sentiment regimes (e.g., contrarian vs. momentum).
* ⏳ **Time Series Stationarity:** Incorporate stationarity tests and model assumptions validation for future forecasting.

---

## 📎 Deliverables

* ✔️ Cleaned and merged dataset
* ✔️ Exploratory and statistical analysis
* ✔️ Predictive modeling (Random Forest)
* ✔️ Visualizations and key metrics
* ✔️ Optimized model via GridSearchCV
* ✔️ Summary report and output image

---


