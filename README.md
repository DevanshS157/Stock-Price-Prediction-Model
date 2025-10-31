# 📈 1-Day Stock-Price Predictor (TATASTEEL.NS)

A clean, beginner-friendly baseline that forecasts **TATASTEEL.NS**'s next-day closing price with classic technical indicators and **Linear Regression**.  
R² = 0.82 on 20 % hold-out, beating a naive walk-forward by > 15 %.  
Everything lives in a single Jupyter notebook—no paid data, no black boxes.

---

## ✅ What you get
* 6-year daily data (yfinance)  
* 8 engineered features (SMA-20, RSI, MACD, lagged prices, etc.)  
* Train / test split respecting temporal order  
* 5-fold **time-series** cross-validation  
* Actual vs. predicted plot + residual diagnostics  
* Re-usable helper functions—drop in any NSE symbol

---

## 🚀 Run in 30 s
```bash
git clone https://github.com/devanshs157/stock-price-prediction-model.git
cd 1day-stock-predictor
pip install -r requirements.txt
jupyter notebook TATASTEEL_1day_predictor.ipynb
```

---

## 📦 Dependencies
```
pandas numpy matplotlib seaborn scikit-learn yfinance
```

---

## 📊 Result snapshot (last fold)
| Metric | Value |
|--------|-------|
| R²     | 0.82  |
| RMSE   | 14.2 INR |

---

## 🤝 Want to improve?
* Swap in XGBoost, LSTM or Facebook Prophet  
* Add more symbols, macro features, or sentiment data  
* Try a multi-horizon target (e.g., +5 days)

PRs welcome—let’s learn together!

---

*Live HTML report* 👉 https://devanshs157.github.io/stock-price-prediction-model/
