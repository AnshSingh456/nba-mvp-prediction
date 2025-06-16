# 🏀 NBA MVP Prediction (2005–2025)

This project uses NBA regular season statistics to predict MVP vote share using machine learning. The model is trained on historical data to forecast the top MVP candidates for the 2023–2024 and 2024–2025 seasons.

---

## 📊 Project Overview

- **Goal**: Predict MVP vote share (`Share`) using player and team statistics
- **Model**: Linear Regression
- **Training Sets**:
  - 2005–2023 for 2024 predictions
  - 2005–2024 for 2025 predictions
- **Evaluation Metrics**: MAE, RMSE, R², Rank evaluation
- **Features Used**: Player stats (e.g., PTS, AST, STL) and team metrics (e.g., W/L%, SRS, PS/G)

---

## 📈 2024 Results (Model trained on 2005–2023)

See `top5_2023-2024.csv` for the top 5 predicted MVP candidates versus actual vote shares.

---

## 📈 2025 Results (Model trained on 2005–2024)

See `top5_2024-2025.csv` for the top 5 predicted MVP candidates versus actual vote shares.

---

## 📁 Files Included

| File                 | Description                                     |
| -------------------- | ----------------------------------------------- |
| `predictor.ipynb`    | Main notebook for training and prediction       |
| `Scrape_NBA.ipynb`   | Scrapes MVP vote data from Basketball Reference |
| `top5_2023-2024.csv` | Predictions vs. actual MVP shares for 2024      |
| `top5_2024-2025.csv` | Predictions vs. actual MVP shares for 2025      |

---

## 📚 Data Source

- Player and team stats, along with MVP voting data, were sourced from [Basketball Reference](https://www.basketball-reference.com/)

---

## 📝 Notes

- Models are trained using only prior years to prevent data leakage
- MVP vote share is treated as a regression target
- Final rankings are derived from predicted shares and evaluated against actual MVP results
