# Pattern-ML Trading Engine
Technical Pattern Signals with Supervised Learning and Backtesting

## Overview
Pattern-ML Trading Engine is a quantitative research project that combines technical pattern recognition, supervised machine learning, and systematic backtesting to optimize trading signal quality. The framework retrieves financial market data, detects and classifies a wide range of candlestick and price-action patterns, evaluates their predictive success, and integrates them into a decision engine for long/short positioning.

The project was initially applied to Apple Inc. (AAPL) equity and progressively expanded to multiple tickers to improve robustness and generalization.

## Key Features

### ✅ Data Retrieval & Visualization
• Automated price-data download from market APIs (e.g. yfinance)  
• Interactive price charts with overlayed indicators and patterns  
• Multi-ticker support for performance optimization

### ✅ Technical Pattern Detection
Patterns classified by structure and context:
• Single-candle formations  
• Multi-candle formations  
• Trend-dependent signals  
• Support/Resistance dependent patterns  
• Volume-based patterns  
• Reversal and continuation patterns  
• Confirmation-driven signals

Patterns are plotted directly on price charts, including bullish/bearish directionality where applicable.

### ✅ Trend Analysis
• Custom trend-detection module  
• Used as a prerequisite for pattern validity  
• Trend labeling for machine-learning feature enrichment

### ✅ Pattern Performance Analytics
• Success-rate computation for each pattern  
• Prediction horizon: from **1 to 20 trading days** after signal appearance  
• Evaluation per full time period or inside specific sub-periods  
• Excel export of aggregated statistics for further research

### ✅ Machine Learning & Backtesting
• Training dataset assembled from detected pattern signals  
• Feature engineering from price, volume, and contextual indicators  
• ML models tested (RandomForest, Gradient Boosting, SVM, Logistic/Linear regression)  
• Backtesting engine to evaluate strategy results based on:
  - Pattern combinations
  - Signal weighting
  - Buy/Sell decision optimization

### ✅ Full Visualization & Reporting
• Unified view overlaying all detected patterns on the price chart  
• Summary dashboards for predictive power and signal reliability

## Technologies & Libraries
• Python: pandas, numpy, scikit-learn, yfinance, matplotlib, seaborn  
• Jupyter Notebook for analysis and prototyping  
• Excel outputs for pattern analytics tracking

## Project Structure