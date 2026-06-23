# Quantitative Multi-Factor Equity Backtesting & Portfolio Optimization

📄 **[Read the Full PDF Report Here](MPAA.pdf)**

## 📌 Project Overview
This project explores factor-based investment strategies on the European market (STOXX Europe 600 universe) from 2015 to 2019. The objective was to design, backtest, and evaluate quantitative strategies combining Value and Quality factors to identify the best risk-adjusted returns.

Due to the use of a proprietary university cloud cluster and backtesting engine (`q.qrumble`), the Python source code is not fully public. This repository hosts the final report detailing the methodology, mathematical modeling, and performance results.

## ⚙️ Methodology
*   **Universe:** STOXX 600 (European Equities).
*   **Time Horizon:** 5-year period (Jan 2015 - Dec 2019) with annual/semi-annual rebalancing.
*   **Strategies Evaluated:** Dogs of the Dow, Joel Greenblatt's Magic Formula, Piotroski's F-Score, and various multi-factor composite models.

## 🚀 Key Findings & Best Strategy
After testing nearly 40 strategy combinations, the highest performing model was a **Multi-Factor Composite Strategy (Quality + Value)**:
1.  **Quality Filter:** Applied the Piotroski F-Score, retaining only companies with a score $\ge 8$.
2.  **Value Filter:** Applied Magic Formula logic (Earnings Yield + Return on Capital), selecting the top 15%.
3.  **Portfolio Construction:** Equal-weighted, annually rebalanced.

### 📊 Performance Metrics (Best Model)
*   **Sharpe Ratio:** 1.14
*   **Cumulative ROI (5y):** +128.42%
*   **Annualized Return:** +17.96%
*   **Alpha:** +47.19%
*   **Beta:** 0.92

## 🛠️ Tech Stack & Skills Demonstrated
*   **Python:** Pandas, Data Manipulation, Time-Series Analysis.
*   **Quantitative Finance:** Factor Investing, Backtesting, Risk Assessment (VaR, Alpha, Beta, Sharpe Ratio), Portfolio Construction.
