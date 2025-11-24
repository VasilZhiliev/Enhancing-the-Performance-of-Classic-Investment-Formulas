# Enhancing-the-Performance-of-Classic-Investment-Formulas

This repository contains the full research code and paper for "Enhancing the Performance of Classic Investment Formulas with Machine Learning" (Vrije Universiteit Amsterdam, MSc Finance & Technology, 2025).

Overview

This study evaluates the application of Machine Learning to modernize four classic systematic investment strategies: Piotroski's F-Score, Greenblatt's Magic Formula, Carlisle's Acquirer's Multiple, and van Vliet & de Koning's Conservative Formula. 
By integrating enhanced value metrics (capitalized R&D expenditure, Operating Cash Flow-to-Price, Net Payout Yield) with XGBoost decision trees, the framework addresses performance decay in traditional rule-based strategies and adapts to evolving market conditions resulting from publication bias.

Model: XGBoost classifier with probabilistic outputs
Data: CRSP & Compustat fundamental and market data (Q1 1980 – Q4 2023)
Features: Formula-specific metrics transformed into quantiles + enhanced value proxies
Target: Probabilistic indicator of quarterly outperformance vs. S&P 500


Key Results:

Out-of-sample period: Q1 2010 – Q4 2023 (14 years, quarterly rebalancing)

ML F-Score: 15.08% CAGR (vs. 9.24% original), Sharpe 0.76 (vs. 0.44), 714.7% cumulative return
ML Magic Formula: 13.56% CAGR (vs. 7.32% original), Sharpe 0.69 (vs. 0.38), 592.8% cumulative return
ML Acquirer's Multiple: 13.30% CAGR (vs. 10.24% original), Sharpe 0.65 (vs. 0.45), 574.1% cumulative return
ML Conservative Formula: 13.20% CAGR (vs. 11.90% original), Sharpe 0.74 (vs. 0.71), 567.0% cumulative return
Combined Strategy: 13.87% CAGR, 217.4% improvement over original combined approach

Statistical Significance: ML F-Score and Combined approach achieve statistically significant Fama-French 5-Factor + Momentum alphas at 1% and 5% levels respectively.
