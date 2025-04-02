# 📈 Advanced Momentum Trading System

A Python-based algorithmic trading system designed to identify and rank stocks with strong short-term momentum using technical indicators, volume analysis, and ensemble ML models. Ideal for trending markets, this system complements mean-reversion strategies and outputs daily stock candidates with confidence scores.

---

## 🚀 Key Features

- **Multi-Timeframe Momentum**: Calculates momentum across short, medium, and long horizons
- **Volume & Volatility Checks**: Confirms breakout strength using volume ratios and volatility normalization
- **Advanced Filtering**:
  - Liquidity and volatility thresholds
  - News sentiment and earnings screening
  - Correlation filters to avoid overexposure
- **ML Scoring System**:
  - Ensemble modeling (Random Forest + XGBoost)
  - Feature importance tracking
  - Probability of continuation scoring
- **Position Sizing**:
  - Volatility-adjusted allocation
  - Correlation-aware portfolio optimization
- **Live Ticker Universe**: Based on S&P 500 constituents (or fallback symbols)

---

## 🧠 Strategy Overview

The system targets stocks demonstrating consistent upward momentum while avoiding false breakouts and high-risk events. It calculates:

- Returns over 5, 10, and 20-day windows  
- RSI (Relative Strength Index)  
- Volume surge ratios  
- Moving average alignment (20 > 50 > price)

Stocks are scored and ranked by a composite momentum score, with optional ML-based confidence modeling.

---

## 🛠️ Tech Stack

- Python 3.11  
- `pandas`, `numpy`, `yfinance`, `scikit-learn`, `alpaca-py`  
- Optional: `xgboost`, `matplotlib`, `seaborn`



